# Task: Stack Overflow -> ret2usr -> SMEP Bypass -> KASLR Bypass -> Full Root Shell

## What you have to do:

Write your own kernel module (`vuln.ko`)
- Creates `/dev/pwn`
- Has an ioctl that does a classic stack buffer overflow 
- hint : (copy >= 256 bytes from userspace into a <= 128-byte stack buffer using `copy_from_user` - no bounds check)
- Overflow must be able to overwrite saved RIP

Set up a QEMU VM with a kernel you compiled yourself (5.15 / 6.1 / 6.8 - your choice)
- Provide the exact `.config` and a script so we can boot your VM in under 10 minutes

## Phase 1 (SMEP = OFF, KASLR = OFF)
Exploit the overflow with normal ret2usr:
- hint: `call commit_creds(prepare_kernel_cred(0))` -> clean return to userspace -> drop a root shell

## Phase 2 (SMEP = ON)
Recompile the kernel with SMEP enabled
- Your Phase 1 exploit will now panic ("SMEP protection fault")
- Fix it by building a ROP chain that:
  - hint: Temporarily disables SMEP (`native_write_cr4` gadget, clear bit 20 of CR4)
  - Escalates privilege
  - Re-enables SMEP before returning to userspace
- Result must be a 100% stable root shell, no kernel panic

## Phase 3 (SMEP = ON, KASLR = ON)
Add proper KASLR bypass by leaking a kernel pointer directly from the overflow (no `/proc/kallsyms`)
- Final exploit works with KASLR + SMEP both enabled

## Success criteria:
- `id` shows `uid=0(root)`
- Kernel stays alive after you exit the shell
- No hardcoded addresses except the ones you leak at runtime


## Evaluation
1. Phase 1 is successful (30%)
2. Phase 2 is successful (30%)
3. Phase 3 is successful (30%)
4. Documentation and code (10%)

## Deliverables
the exploit
