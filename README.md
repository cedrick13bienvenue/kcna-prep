# Kubernetes and Cloud Native Associate (KCNA) example questions

**What core principle of cloud-native application delivery emphasizes treating infrastructure components and application deployments as disposable units replaced on update?**

- A. Statefulness
- B. Mutability
- C. Immutability
- D. Manual Configuration
- E. High Cohesion

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**In GitOps, what serves as the single source of truth for the desired state of the application and infrastructure?**

- A. The running cluster state queried via kubectl.
- B. A configuration management database (CMDB).
- C. A Git repository containing declarative configuration manifests.
- D. A wiki page maintained by the operations team.
- E. The CI/CD pipeline logs.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is the primary goal of Continuous Integration (CI) in a CI/CD pipeline?**

- A. To automatically deploy every code change directly to production..
- B. To frequently merge code changes into a central repository and automatically build and test the application.
- C. To manage the Git repository permissions for developers.
- D. To provision the underlying infrastructure required for deployment.
- E. To manually review code quality before merging.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**How does the declarative nature of Kubernetes manifests support cloud-native application delivery principles?**

- A. By requiring developers to specify exact imperative commands for deployment.
- B. By allowing users to define the desired state, leaving the how to the orchestrator's control loop.
- C. By enforcing the use of specific programming languages for applications.
- D. By automatically generating Git repositories for each application.
- E. By integrating directly with billing systems for cost management.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**What is the role of a GitOps agent or operator (like Argo CD or Flux) running within the Kubernetes cluster?**

- A. To build container images from source code committed to Git.
- B. To run automated tests against application code in Git.
- C. To continuously monitor the Git repository and reconcile the cluster state to match the desired state in Git.
- D. To provide a web UI for developers to manually apply manifests to the cluster.
- E. To manage user access control to the Git repository.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---
