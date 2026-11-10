---
title: "Learning Matches for Mesh Deformation via REINFORCE"
excerpt: "Co-designed a new mesh deformation pipeline in which points correspondences are learned as a policy.  <br/><img src='/images/cvlab_logo.png'>"
collection: portfolio
---
[📄 Report (PDF)](/files/RL_Project__Report.pdf) | [💻 Code](https://github.com/denizmsayin/rl-mesh-deformation)

Template-based mesh deformation is widely used in geometric deep learning and
medical image analysis, where an initial source mesh is iteratively deformed to
match a target shape. Standard pipelines usually rely on Chamfer distance, that can
behave poorly as an optimization objective producing fragile correspondences and
many-to-one vertex collapse. This project investigates whether point correspondences
can instead be learned as a policy for iterative regularized deformation. We
formulate mesh matching as a reinforcement learning problem, trying to learn a
neural policy that can predict matches based on input shapes, in which the state is
the current source-target configuration, the action is a correspondence proposal, the
transition is represented by deformation steps, and the reward is the final fit quality.
The REINFORCE algorithm allows us to optimize this discrete matching policy
with policy gradients. As directly starting with 3D is challenging both technically
and computationally, we begin with a simplified 2D environment using procedurally
generated shapes, then compare the learned policy against nearest-neighbor
Chamfer matches. We illustrate improvements and discuss various trade-offs, design
choices and possible extensions supported by experiments.