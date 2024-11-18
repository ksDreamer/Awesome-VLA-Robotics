# Awesome-VLA-Robotics
A list and my notes about VLA(Vision Language Model) on Robotics.  

There are more and more work utilizing Language Model's power to enhance robot's ability. While the basic executation ability(low level aspect) such as actuator and electicity is independent, the perception and planning ability(high level aspect) such as sensing and task arrangement can be highly updated by VLA.  TODO: What about the middle layers(locomotion, manipulation)? What is the deviding principle.  
Aside, in motion planning and control field, the RL-based method is having more and more attention than traditional dynamics and kinematic model based control method.
The VLA here is a big topic, containing LLM(Large Language Model), VLM(Vision Language Model), VLA(Vision Language Action), FM(Foundation Model), LVM(Large Vision Model), etc.


Following are the list and my notes.

[SayCan](https://say-can.github.io) by Google Deepmind, 2022
* [[paper](https://say-can.github.io/assets/palm_saycan.pdf)] | [[code](https://github.com/google-research/google-research/tree/master/saycan)]
* The very first project utilizing LLM and VLM to plan robot tasks. It introduced a planning framework combining LLM semantic understanding and vision perception of affordance.

[RT-2](https://robotics-transformer2.github.io) by Google Deepmind, 2023
* [[paper](https://robotics-transformer2.github.io/assets/rt2.pdf)]
* Developed from previous [RT-1](https://robotics-transformer1.github.io)(simple LLM planning) and PaLM-E(LLM with knowledge from robotics field)
* A great work for robotics. Inspired from SayCan and RT-2, we have many works in robot leanrning, manipulation and perception. Later we have Open-X Embodiment dataset and RT-X project.

[ReKep](https://rekep-robot.github.io) by Standford Feifei Li, 2024
* [[paper](https://arxiv.org/abs/2409.01652)] | [[code](https://github.com/huangwl18/ReKep)]
* Using LVM(large vision model) such as [dinov2](https://ai.meta.com/blog/dino-v2-computer-vision-self-supervised-learning/) and [sam2](https://ai.meta.com/sam2/), combined with VLM(Vision Language Model) such as [GPT-4o](https://openai.com/index/hello-gpt-4o/), to generate constraint, so as to plan robot manipulation tasks.
* Constraints: 1. candidate keypoint for manipulation. 2. sub-goal constraint for multi-tasks 3. path constraint for space-varying and pose-demanding tasks





---
TODO: Diffusion Policy, Cheng-Chi, Diffusion model on Robotics.





