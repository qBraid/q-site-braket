# Q-SITE Hackathon qBraid-AWS Challenge

**Optimizing Quantum Approximate Optimization Algorithm (QAOA) for Weighted Max-k-Cut Using Amazon Braket**

## **Challenge Overview:**

In this challenge are tasked with implementing and optimizing the **Quantum Approximate Optimization Algorithm (QAOA)** to solve the **Weighted Max-K-Cut problem**. The goal is to achieve high-quality solutions while optimizing for execution cost and performance using Amazon Braket. We're looking to test your teams ability to design quantum algorithms, perform circuit optimization, and utilize real quantum hardware efficiently.

---
The **Weighted Max-k-Cut** problem is a generalization of the Max-Cut problem. Given a graph \( G = (V, E) \) where each edge has an associated weight \( w_{ij} \), the goal is to partition the vertices \( V \) into \( k \) subsets in such a way that the sum of the weights of edges between different subsets is maximized.

Participants will:

1. **Formulate the Weighted Max-k-Cut problem** as a binary optimization problem.
2. **Implement the QAOA** algorithm using Amazon Braket to solve this problem.
3. **Optimize QAOA** for performance, circuit depth, accuracy, and execution cost.
4. **Experiment with various quantum hardware backends** (e.g., Rigetti, IonQ, or IQM) and simulators such as SV1 to compare performance and scalability. We highly encourage you to run your solution with a local simulator before running it on real devices or cloud simulators.

### Using qBraid for development
Fork this repository into your account, and copy its git clone url e.g. https://github.com/<user>/q-site-braket.git. 

At the bottom of this README in the forked repo, click the Launch on qBraid button to clone this repository and launch qBraid Lab.

Open terminal (first icon in the Other column in Launcher) and cd into the `q-site-braket` repo. Set the repo's remote origin using the git clone url you copied in Step 1, and then create a new branch for your team:

cd q-site-braket
git remote set-url origin <url>
git branch <team_name>
git checkout <team_name>
Use the environment manager (ENVS tab in the right sidebar) to install environment "Amazon Braket 1.86". The installation should take ~2 min.

---

## **Challenge Goals:**

1. **Implementation of QAOA**: 
   - Implement the QAOA algorithm to solve the Weighted Max-k-Cut problem for different graphs and values of \( k \).
   - Use Amazon Braket’s SDK for the implementation, including simulations and real hardware executions.
   - Use qBraid SDK to submit your Amazon Braket circuit to a backend. If you need credits please let us know!

2. **Optimization**:
   - Optimize the QAOA circuit by minimizing gate depth and maximizing the accuracy of the solution.
   - Perform classical parameter optimization for the angles in the QAOA algorithm using gradient-based or heuristic methods.

3. **Hardware Comparison**:
   - Execute the QAOA algorithm on at least two quantum hardware backends (e.g. at least two of Rigetti, IonQ, or IQM) and compare performance using the qBraid SDK.
   - Analyze metrics such as gate count, execution time, solution quality, and hardware noise resilience. 

4. **Error Mitigation**:
   - Implement and test at least one error mitigation strategy to improve the quality of results when using real quantum hardware.

---

## **Deliverables:**

1. **Code Repository**:
   - Fork this repository and submit your code on GitHub by creating a pull request so we can view your results! 
   - Make sure to include clear instructions on how to run the experiments and reproduce your results.
   - The code should be modular and well-documented, if we can't run the code, we can't validate your results!!!

2. **Final Report**:
   - Include everything in one jupyter notebook runnable on qBraid with the [Amazon Braket (1.86) ](https://docs.qbraid.com/lab/user-guide/environments#install-environment) environment.
    <img src="./amazon_braket_v186.png" width="200px" style="margin: auto;">

   - Detailed report in the jupyter notebook explaining your implementation, including the formulation of the Weighted Max-k-Cut problem and QAOA.
   - Discuss the optimization techniques used, the results obtained, and the comparison of hardware backends.
   - Include insights into the performance of your QAOA as \( k \) increases.

3. **Cost Analysis**:
   - Include a breakdown of quantum resource usage, including the number of shots, execution time, and gate complexity for each hardware backend.
   - Describe the strategies used to minimize the cost of running your experiments on Amazon Braket. Comments or markdown cells with explanations above or below the implementation is acceptable.

---

## **Evaluation Criteria**:

1. **Technical Implementation (40%)**:
   - Correctness of the QAOA implementation for the Weighted Max-k-Cut problem.
   - Efficient use of Amazon Braket’s SDK and quantum hardware.
   - Circuit optimization quality, including gate depth and resource usage.
   - Code cleanliness, the code should be well modularized and well documented.

2. **Optimization and Performance (30%)**:
   - Success in optimizing the algorithm for both accuracy and cost.
   - Effective parameter tuning and hardware optimization.
   - Quality of results compared to classical methods (optional bonus benchmark).

3. **Analysis and Insights (20%)**:
   - Depth of the analysis presented in the final report.
   - Insights into the trade-offs between cost, execution time, and solution quality.
   - Understanding of how quantum hardware limitations (noise, qubit connectivity) affect the performance.

4. **Documentation and Presentation (10%)**:
   - Clear, well-organized documentation of code and results.
   - Quality of the final presentation and report, including visualizations and explanations of key insights.
---
## Prize

The first prize team will be awarded qBraid credits to further test their solution on ionq devices.

---

## Working on qBraid
[<img src="https://qbraid-static.s3.amazonaws.com/logos/Launch_on_qBraid_white.png" width="150">](https://account.qbraid.com?gitHubUrl=https://github.com/qbraid/q-site-braket.git)
1. To launch the challenge on qBraid, click the above `Launch on qBraid` button. It will take you to your qBraid Lab with the repository cloned.


For other questions or additional help using qBraid, see [Lab User Guide](https://docs.qbraid.com/en/latest/), or reach out on the qBraid Slack channel.


## References
- [Efficient encoding of the weighted MAX k-CUT on a quantum computer using QAOA](https://arxiv.org/pdf/2009.01095)

- [Amazon Braket](https://aws.amazon.com/braket/)

- [qBraid SDK](https://github.com/qbraid/qbraid)
