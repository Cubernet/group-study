**Title:** Fast Is Better Than Free: Revisiting Adversarial Training

**Source:** ICLR 2020

**Authors:** Eric Wong,Leslie Rice,J. Zico Kolter

---

**Summary**

This work find a special adversarial training approach:FGSM adversarial training with random initialization, by using this approach to train model, the model can be as effective as the model trained by PGD adversarial training while having lower cost.

---

**Strengthens**  

- Speed up adversarial training without compromising the model robustness.

- A variety of accelerated training methods are listed in this article for our reference.

---

**Weaknesses**  

- The theoretical proof of the random initialization method proposed in this paper is lacking.
- The effect of iteration was not considered in the ablation experiments with Free FGSM.
---

