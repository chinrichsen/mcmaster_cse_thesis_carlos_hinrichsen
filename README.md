# 🚚📚 Vehicle Routing Problem with Interdiction (VRPI)

Welcome to the repository for my master’s thesis, **“A Meta-Heuristic Algorithm for Vehicle Routing Problem with Interdiction”**. This project studies how to solve vehicle routing problems when routes may become unusable due to interdiction events such as natural disasters, infrastructure failures, conflict, or other disruptions. 🌍⚠️

The repository includes benchmark data, small test instances, interdiction probabilities, and replication materials related to the thesis and Xu (2017). 🧩

---

## ✨ Overview

This research focuses on the **Vehicle Routing Problem with Interdiction (VRPI)**, an extension of the classic Vehicle Routing Problem where some routes may be blocked or interrupted with a certain probability. The thesis compares **exact methods** using **CPLEX** with **heuristic methods** based on **GRASP** (Greedy Randomized Adaptive Search Procedure). 🧠🚛

The work also develops a flexible framework that can be adapted to:

- **CVRP**: Capacitated Vehicle Routing Problem.
- **SDVRP**: Split Delivery Vehicle Routing Problem.
- **VRPI**: Vehicle Routing Problem with Interdiction.

It further introduces improvements over the original Xu (2017) implementation, including:

- Large benchmark instance support.
- A more flexible GRASP framework.
- A 3-fold decision logic for route selection.
- Minimum-demand logic.
- Parameter calibration for better solution quality. 🔧📈

---

## 🎯 Research Goal

The main goal of this thesis is to answer the following question:

**How can routing plans be built efficiently and robustly when routes may be interdicted?**

To address this, the thesis:

- Models route risk using interdiction probabilities.
- Tests feasibility and solution quality under different scenarios.
- Compares exact and heuristic approaches.
- Extends the analysis to benchmark instances and larger problem sizes. 🛣️

---

## 🧪 Methods Used

This project uses a mix of optimization and metaheuristic techniques:

- **CPLEX** for exact optimization on small instances. 🧮
- **GRASP** for heuristic and scalable solution generation. ⚙️
- **K-Nearest Neighbors (KNN)** for initial route construction in some configurations. 🧭
- **Local search** improvements such as:
  - 2-opt
  - 3-opt
  - swap
  - segment reversal 🔁
- **Parameter calibration** to improve performance across different instance types. 🎛️

The thesis also studies:

- Feasibility under tight capacity constraints.
- The impact of interdiction probabilities.
- The trade-off between minimizing cost, minimizing interdiction risk, and satisfying demand. ⚖️

---

## 📁 Repository Structure

Based on the current folder structure, the repository contains:

- **Interdiction Probabilities Benchmark Instances**  
  Contains interdiction probability data for benchmark-sized instances. 📊

- **Interdiction Probabilities Small Instances**  
  Contains interdiction probability data for small test instances. 🧪

- **VRPI CPLEX Small Instances with and without Interdiction**  
  Contains exact-solver results for small instances, comparing cases with and without interdiction. ✅

- **VRPI GRASP Benchmark Instances**  
  Contains heuristic results for benchmark instances using the GRASP approach. 🚀

- **VRPI GRASP Small Instances with and without Interdiction**  
  Contains GRASP results for small instances under different interdiction settings. 🔎

- **Xu 2017 Replicating Results**  
  Contains replication material related to Xu (2017). 📄

---

## 🧭 How to Use This Repo

A simple way to explore the repository is:

1. Start with the **Xu 2017 Replicating Results** folder to understand the baseline work.
2. Review the **small instances** folders to see exact and heuristic comparisons.
3. Check the **benchmark instances** folders to inspect the larger-scale GRASP experiments.
4. Look at the interdiction probability folders to understand how route risk is represented. 🗂️

If you are trying to reproduce the thesis results, the small instances are the best starting point because they are easier to validate against exact solutions. Then you can move to benchmark instances to test scalability. 📚

---

## 📌 Key Contributions

This thesis contributes several important improvements to the VRPI literature:

- A broader and more flexible GRASP framework. 🛠️
- A 3-fold route selection logic that considers:
  - travel cost,
  - interdiction probability,
  - minimum-demand satisfaction. 🎯
- Better handling of capacity and infeasibility issues.
- Extension from small random instances to benchmark instances.
- A clearer and more reproducible experimental setup. 🔬

These contributions make the approach more practical for high-risk logistics, humanitarian delivery, and other uncertain routing environments. 🚨🚚

---

## 📊 Main Findings

The thesis shows that:

- Interdiction can significantly affect feasibility and solution quality.
- Tight capacity and demand settings make VRPI especially sensitive.
- GRASP can perform well on both small and larger benchmark instances.
- Considering minimum demand under interdiction is important for avoiding weak solutions.
- Exact methods like CPLEX are useful for validation on small cases, but heuristics are necessary for larger ones. 📉📈

---

## 🧾 Citation

If you use this repository or reference this work, please cite the thesis:

**Carlos E. Hinrichsen Picand**  
*“A Meta-Heuristic Algorithm for Vehicle Routing Problem with Interdiction”*  
Master of Science Thesis, McMaster University, 2024. 🎓

If you also want to acknowledge the baseline work, cite:

- **Xu (2017)** for the original VRPI formulation and early GRASP approach. 📖

---

## 🔐 Notes

- Some models and implementation details may be available upon request, depending on the thesis distribution policy. 📬
- This repository is intended for research, experimentation, and reproducibility.
- Folder names and contents may continue to evolve as the project is organized. 🧱

---

## 🤝 Acknowledgements

I would like to thank my supervisor, **Dr. Kai Huang**, for his guidance and support throughout this research. I also want to thank my wife and children for their patience, encouragement, and support during the completion of this work. ❤️

---

## ⭐ Final Remark

This repository documents a thesis project that combines **optimization**, **metaheuristics**, and **real-world routing uncertainty** into one reproducible research workflow. It is especially relevant for logistics, humanitarian operations, and other high-risk transportation settings. 🌐
