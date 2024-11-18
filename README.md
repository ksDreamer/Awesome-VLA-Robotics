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
* Developed from previous [RT-1](https://robotics-transformer1.github.io)(an efficient Transformer-based architecture designed for robotic control) and PaLM-E(LLM), RT-2 is a large vision-language model co-fine-tuned to output robot **actions** as natural language tokens.
* A great work in robotics. Later we have [Open-X Embodiment](https://robotics-transformer-x.github.io) project and RT-X dataset.

From SayCan and RT-2 on, we have many excellent work using VLA in robot learning, manipulation and perception.

For example, Stanford, Feifei Li's lab has proposed lots of work about vision and spatial intelligence in robotics manipulation tasks. Here are some:

[VoxPoser](https://voxposer.github.io), CoRL 2023 (Oral)
* [[paper](https://arxiv.org/abs/2307.05973)] | [[code](https://github.com/huangwl18/VoxPoser)]
* label affordances and constraints in 3D perceptual space for zero-shot robot manipulation in the real world.

[ReKep](https://rekep-robot.github.io), CoRL 2024 (Best Paper)
* [[paper](https://arxiv.org/abs/2409.01652)] | [[code](https://github.com/huangwl18/ReKep)]
* Using LVM(large vision model) such as [dinov2](https://ai.meta.com/blog/dino-v2-computer-vision-self-supervised-learning/) and [sam2](https://ai.meta.com/sam2/), combined with VLM(Vision Language Model) such as [GPT-4o](https://openai.com/index/hello-gpt-4o/), to percept input(semantic and vision), generate constraint, **finally plan tasks for robot manipulation**.
* Constraints: 1. candidate keypoint for manipulation. 2. sub-goal constraint for multi-tasks 3. path constraint for space-varying and pose-demanding tasks





---
TODO: Diffusion Policy, Cheng-Chi, Diffusion model on Robotics.





