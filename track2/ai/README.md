# Adversarial Attacks on Artificial Intelligence


We assume you are interested in machine learning and artifiical intelligence, and have a prior background as well, in these topics. In case you don't, then we suggest you to spend the first week or so in a rigorous schedule of learning preliminary concepts crucial to proceed, such as what a [transformer](https://arxiv.org/pdf/1706.03762) is. Keep in mind, these are not designed to be easy (our club members also have a hard time with these), so don't fret if it doesn't come to you all in the first time you read it. These assignments are open-ended, and the goal firstly, it to establish proper foothold in these areas so once you join the club, you are already acquainted with what's hot in the area and how to go from ideation to implementation, and secondly, to make valuable research contributions to the scientific and security community at large. 

This is a very research heavy task, and maybe you will appreciate this website for [finding relevant literature](https://www.connectedpapers.com/) 
Successfully implementing a new attack will mean you're practically in the club, while implementing a black-box attack will mean you're a legend, and you should submit your paper to BlackHat.

## Assignment A - Leveraging mechanistic interpretability for adverarial attacks

Mechanistic interpretability was a term coined by [Chris Olah](https://colah.github.io/about.html). The goal was to understand how neural networks, especially LLMs function on the inside, since they're essentially a black-box. Finding out how LLMs decide what to do, and how, is a major open problem in [aligning LLMs](https://www.turing.com/resources/llm-alignment-and-safety-guide). [Recent strides](https://arxiv.org/pdf/2501.16496) have made it possible to dig deeper, and develop probes into reversing neural networks.

One novel use case is to use interpretability techniques to develop attacks against LLMs. A [recent paper](https://arxiv.org/pdf/2503.06269) sucessfully demonstrated the same, achieving an attack success rate (ASR) of up to 95% against models such as Gemma 2, Llama 3.2, and Qwen 2.5.

Your task is to encome up with new ways to leverage interpretability that can perform white-box or black-box attacks on LLMs. Llama/Qwen (3+) are appropriate targets. 
This can be really daunting, and we understand. Try following along the [ARENA book](https://github.com/callummcdougall/ARENA_3.0), it's literally tailor made for AI safety research.
### Evaluation

1. Understanding of basic concepts in ML - CNNs, backpropagation, etc. [20%]
2. Knowing how transformers work and what circuits are [20%]
3. Researching and implementing existing attacks [30%]
4. Coming up with novel attacks [30%]

## Deliverables

For 1 and 2, the evaluation will be mainly verbal, but for 3 and 4, an academic paper-style report is required that comparatively details what attacks were tried out, their ASRs, and the new attacks implemented. All code, weights and data should be released publically, and the links for the same must be embedded in the report. The attacks must be fully reproducible, and ideally a Dockerfile should be included that sets up and end-to-end pipeline, from downloading any weights, to evaluating the attacks. Use [Harmbench](https://github.com/centerforaisafety/HarmBench) for evaluation.

If your works leads you somewhere, consider applying to [Neel Nanda](https://www.neelnanda.io/)'s [MATS Program](https://www.matsprogram.org/).

## Assignment B - Targeted adversarial attacks on Vision-Language Models

Until late 2010s, object detection was dominated by CNNs, such as ResNet and AlexNet. As of late(>2021), [ViT](https://arxiv.org/pdf/2010.11929)s have begun to dominate, with the emergence of models such as [CLIP](https://arxiv.org/pdf/2103.00020). Thus, adversarial attacks have also become harder, moving away from [FGSM attacks](https://adversarial-ml-tutorial.org/adversarial_examples/) to more complex, multi step attacks such as [this one](https://arxiv.org/pdf/2410.05346). At the core, they're all just adversarial noise perturbation....because...yes...if you read the description for Assignment A, then you know that its coz we just dont get how these neural networks stuff works inside.

While our comrades try to understand and attack models via interpretability, you take the other route. Your goal is...yes.. increase the ASR on adversarial attacks on VLMs. Vision Language Models have become extremely popular, and we have achieved a [great progress in robotics](https://www.pi.website/blog/pistar06) due to them. Imagine if a robot thought a baby was a mosquito, and a knife a swatter. These consequences would be catastrophic. (and someone people have [already tried it](https://arxiv.org/pdf/2506.03350)) Set aside the feasibility of them (how do you hack the robot's camera' etc) and realize that we live in a time of great wonder and danger.

## Evaluation

1. Understanding of basic concepts in ML - CNNs, backpropagation, etc. [20%]
2. Knowing how transformers work and what ViTs are [20%]
3. Researching and implementing existing attacks [30%]
4. Coming up with novel attacks [30%]

## Deliverables

For 1 and 2, the evaluation will be mainly verbal, but for 3 and 4, an academic paper-style report is required that comparatively details what attacks were tried out, their ASRs, and the new attacks implemented. All code, weights and data should be released publically, and the links for the same must be embedded in the report. The attacks must be fully reproducible, and ideally a Dockerfile should be included that sets up and end-to-end pipeline, from downloading any weights, to evaluating the attacks. Use the AnyAttack paper linked above as a starting point for benchmarks and evaluation.
