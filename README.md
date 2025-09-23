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

**What distinguishes Continuous Delivery from Continuous Deployment within a CI/CD pipeline?**

- A. Continuous Delivery involves manual testing; Continuous Deployment is fully automated.
- B. Continuous Delivery deploys to production automatically; Continuous Deployment requires manual approval.
- C. Continuous Delivery ensures code is always deployable; Continuous Deployment automatically deploys it.
- D. Continuous Delivery focuses on infrastructure; Continuous Deployment focuses on application code.
- E. Continuous Delivery uses Git; Continuous Deployment uses SVN.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**Why is a feedback loop important in cloud-native application delivery?**

- A. It eliminates the need for version control systems like Git.
- B. It ensures that only senior developers can deploy applications.
- C. It provides visibility into the deployment process and application health, enabling quick response to issues.
- D. It mandates the use of specific cloud providers for hosting.
- E. It replaces the need for automated testing.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**In the "pull-based" GitOps model, where does the initiative for updating the cluster state originate?**

- A. The CI server pushes changes directly to the Kubernetes API server.
- B. The developer manually runs kubectl apply from their workstation.
- C. The GitOps operator running inside the cluster pulls changes from the Git repository.
- D. An external webhook triggers the update based on Git commits.
- E. The Git repository pushes changes directly to the cluster nodes.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is the primary function of a container registry (e.g., Docker Hub, Google Container Registry, Harbor) in the CI/CD process?**

- A. To store source code repositories.
- B. To run automated unit and integration tests.
- C. To store and distribute container images built by the CI process.
- D. To host Kubernetes manifest files declaratively defining deployments.
- E. To manage DNS records for deployed applications.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---
