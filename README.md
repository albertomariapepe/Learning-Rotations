
# Learning Rotations 🌀

Mathematical Methods in the Applied Sciences / AGACSE 2021


**Citation:**

```bibtex
@article{pepe2024learning,
  title={Learning rotations},
  author={Pepe, Alberto and Lasenby, Joan and Chac{'o}n, Pablo},
  journal={Mathematical Methods in the Applied Sciences},
  volume={47},
  number={3},
  pages={1204--1217},
  year={2024},
  publisher={Wiley Online Library}
}
```

## Introduction 📑

In the field of **computer vision** 🤖, tasks such as **pose estimation** from images 📸 or 3D point clouds 🌐 are central to many advancements. These problems often involve learning **rotations**, which is a fundamental aspect of these tasks. However, there is no universally accepted method for parametrizing rotations mathematically. Different representations such as matrices, quaternions, Euler angles, and axis-angle are commonly used, but each of them comes with its own limitations, including **gimbal lock**, **discontinuities**, and **antipodal symmetry** 🌀. These issues can complicate the training of **neural networks**, potentially leading to significant errors.

This paper proposes a solution by utilizing a **geometric algebra (GA)** description of rotations. This approach is compared with a **6D continuous representation**, and we show that it not only resolves the limitations of previous methods but also **outperforms** them in terms of **regression accuracy** and **robustness to noise**. In this process, we present three detailed case studies that demonstrate the effectiveness of GA in solving these complex problems.

## Case Studies 💡

In line with recent literature, we introduce three case studies to illustrate the practical application of GA in rotation learning:

1. **A sanity check** ✅ – Testing the performance of the proposed method in controlled scenarios to validate its robustness.
2. **Pose estimation from 3D point clouds** 🌐 – A real-world scenario where GA is applied to estimate poses from 3D data.
3. **An inverse kinematic problem** 🦾 – Using GA to solve inverse kinematics for robotic systems, showcasing its utility in practical engineering applications.

For each case study, we employ the **GA formulation** of rotations and compare it with the **6D continuous representation** previously presented in the literature. The findings demonstrate that **parametrizing rotations as bivectors** significantly improves upon the 6D representation by requiring fewer parameters and offering better **generalizability**.

## Why Geometric Algebra? 🤔

Geometric Algebra (GA) offers several advantages over traditional rotation representations:
- **Continuity**: GA avoids the continuity issues seen with other representations, such as 6D.
- **Efficiency**: GA requires fewer parameters, making it more efficient to train neural networks for regression tasks.
- **Robustness**: GA provides enhanced resilience to noise, ensuring better performance in **high-noise scenarios** 🎯.

Our empirical results show that GA provides a **simple**, **compact**, and **effective** framework for describing rotations in a manner well-suited to deep learning tasks. This approach not only achieves high regression accuracy but also exhibits strong generalizability across various conditions.

## Code & Datasets 📊

The code to generate and process the datasets is available in the **notebooks**, allowing others to replicate and build upon this work. The **ready-to-use datasets** can be obtained from the authors upon request 📩.

---

This paper provides a comprehensive exploration of how **Geometric Algebra** can be applied to rotation learning, showcasing its practical advantages in various real-world applications. 

