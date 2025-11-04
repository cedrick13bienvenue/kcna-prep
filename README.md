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

**What cloud-native delivery concept involves gradually shifting traffic from an old version of an application to a new version while monitoring performance?**

- A. Blue/Green Deployment.
- B. Rolling Update.
- C. Canary Release.
- D. A/B Testing.
- E. To manage DNS records for deployed applications.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

---

**What benefit does GitOps provide regarding auditability and rollback?**

- A. It eliminates the need for logging application events.
- B. It relies on manual documentation stored outside Git for tracking changes.
- C. Every change to the desired state is a Git commit, providing a full audit trail and easy rollback via git revert.
- D. Rollbacks must be performed by directly modifying the live cluster state.
- E. Audit trails are only available through proprietary third-party tools.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

---

**In a typical Kubernetes CI/CD pipeline, what stage usually occurs immediately after building the container image?**

- A. Deploying the image to the production Kubernetes cluster.
- B. Pushing the container image to a container registry.
- C. Running end-to-end tests requiring a fully deployed environment.
- D. Manually approving the release for deployment.
- E. Configuring DNS records for the new application version.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

---

**Which deployment strategy involves running two identical production environments, only one of which receives live traffic at any time?**

- A. Canary Release.
- B. Rolling Update.
- C. Blue/Green Deployment.
- D. Shadow Deployment.
- E. Recreate Deployment.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**How does the concept of "configuration drift" relate to GitOps?**

- A. GitOps intentionally introduces configuration drift for flexibility.
- B. Configuration drift is the desired outcome of a GitOps workflow.
- C. GitOps aims to prevent or automatically correct configuration drift by continuously reconciling the cluster state with Git.
- D. Configuration drift refers to changes made only within the Git repository.
- E. GitOps requires manual intervention to detect configuration drift.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What role does automated testing (unit, integration, end-to-end) play in achieving reliable Continuous Delivery/Deployment?**

- A. It slows down the delivery pipeline unnecessarily.
- B. It provides the confidence needed to automate deployments by verifying application correctness at different levels.
- C. It is only necessary for applications written in specific languages.
- D. It replaces the need for monitoring and observability post-deployment.
- E. It primarily focuses on testing the underlying Kubernetes infrastructure.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**Which practice aligns best with the principle of using declarative specifications for application delivery?**

- A. Writing shell scripts that execute a series of kubectl commands to deploy.
- B. Using Kubernetes manifests (YAML) stored in Git to define the desired application state.
- C. Manually configuring applications through a graphical user interface after deployment.
- D. Storing application configuration directly within container images.
- E. Using SSH to log into nodes and manually start application processes.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**What is a potential challenge or consideration when implementing GitOps?**

- A. It makes rollbacks significantly more difficult than traditional methods.
- B. It requires developers to have direct kubectl apply access to production clusters.
- C. Managing secrets securely within a Git-based workflow requires careful handling (e.g., using sealed secrets, external secret managers).
- D. It eliminates the need for any CI pipeline processes like building and testing.
- E. It only works with specific proprietary Git hosting providers.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is "pipeline-as-code" in the context of CI/CD?**

- A. Writing application code directly within the CI/CD tool's UI.
- B. Defining the CI/CD pipeline's stages, steps, and configuration using code stored in version control (e.g., Jenkinsfile, GitLab CI YAML).
- C. Generating pipeline definitions automatically based on monitoring data.
- D. A specific programming language used exclusively for writing CI/CD pipelines.
- E. Storing pipeline execution logs as application code.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**How does the concept of "least privilege" apply to GitOps operators?**

- A. The operator should run with cluster-admin privileges for maximum flexibility.
- B. The operator's permissions (e.g., via ServiceAccount and RBAC) should be scoped only to the resources it needs to manage.
- C. Developers interacting with Git should have least privilege; the operator needs full access.
- D. The operator should only have read-only access to the Git repository.
- E. Least privilege only applies to CI/CD tools, not GitOps operators.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**What is the purpose of tools like Helm or Kustomize in Kubernetes application delivery?**

- A. To replace the need for container image registries.
- B. To provide runtime monitoring and alerting for applications.
- C. To manage, template, and customize Kubernetes manifest files, simplifying complex deployments.
- D. To automatically write application source code based on high-level requirements.
- E. To enforce network security policies between Pods.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**In a GitOps workflow, how are changes typically promoted across different environments (e.g., staging to production)?**

- A. By directly modifying the live production cluster using kubectl.
- B. By manually copying manifests from a staging directory to a production directory on a local machine.
- C. By merging or promoting changes between branches or directories in the Git repository that represent different environments.
- D. By re-running the entire CI pipeline with a "production" flag.
- E. By configuring the GitOps operator to ignore environment differences.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is the significance of using unique, immutable tags (e.g., Git SHA, semantic version) for container images in a CI/CD pipeline?**

- A. It allows developers to overwrite existing tags like latest for simplicity.
- B. It makes it difficult to track which version of the code is running in production.
- C. It ensures that deployments are predictable and repeatable, always pulling the exact intended version of the image.
- D. It reduces the storage space required in the container registry.
- E. It is primarily for aesthetic purposes in dashboard displays.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is a key benefit of automating application delivery pipelines?**

- A. It increases the need for manual intervention and approvals at each stage.
- B. It introduces more opportunities for human error during deployment.
- C. It leads to faster, more reliable, and consistent deployments, enabling quicker feedback loops.
- D. It makes the deployment process less transparent and harder to audit.
- E. It primarily benefits only very small development teams.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**If a discrepancy exists between the state defined in Git and the live cluster state, what is the expected behavior of a GitOps reconciliation loop?**

- A. It sends an alert to the developer asking them to manually fix the cluster.
- B. It automatically updates the Git repository to match the cluster state.
- C. It detects the drift and takes action to modify the cluster state to match the desired state in Git.
- D. It halts all further deployments until the discrepancy is manually resolved.
- E. It ignores the discrepancy unless explicitly told to sync.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What security practice should be integrated into a CI pipeline dealing with container images?**

- A. Disabling all network access for the CI runner.
- B. Storing plain-text API keys directly in the pipeline script.
- C. Scanning container images for known vulnerabilities (CVEs) using tools like Trivy, Clair, or Snyk.
- D. Granting the CI runner root privileges on the build host.
- E. Bypassing all automated tests to speed up the build process.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**Which component is typically NOT considered part of a core GitOps workflow?**

- A. A Git repository containing declarative manifests.
- B. An automated mechanism to apply changes from Git to the cluster (Operator).
- C. A mechanism to observe the cluster state and compare it with Git (Operator).
- D. An imperative script run manually by developers to deploy applications.
- E. A feedback mechanism reporting synchronization status.

<details><summary>Answer</summary>

**Correct answer:** D

</details>

---

**In CI/CD for Kubernetes, why is it often better to update the image tag in a deployment manifest rather than using the latest tag?**

- A. Using latest triggers automatic rollbacks on failure.
- B. The latest tag provides better caching performance in the container registry.
- C. Updating a specific tag declaratively triggers a controlled rollout; latest doesn't reliably signal updates.
- D. The latest tag is not supported by most container registries.
- E. Using specific tags requires less storage space in Git.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What does "Shift Left" mean in the context of security in application delivery?**

- A. Moving security testing and considerations to the rightmost (production) stage of the pipeline.
- B. Integrating security checks and practices earlier in the development lifecycle (e.g., in CI).
- C. Assigning all security responsibilities solely to a dedicated security team.
- D. Ignoring security concerns until after an application has been deployed.
- E. Focusing security efforts only on the underlying infrastructure.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**Can GitOps manage resources outside of Kubernetes (e.g., cloud databases, DNS records)?**

- A. No, GitOps is strictly limited to managing Kubernetes API objects.
- B. Yes, potentially, if using tools like Crossplane or Terraform controllers that extend the GitOps model to manage external resources.
- C. Only if the external resources are manually synchronized with Git state.
- D. No, managing external resources always requires a separate imperative process.
- E. Yes, by storing credentials for cloud providers directly in Git manifests.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**What is the purpose of a "smoke test" in a CD pipeline, often run immediately after deployment?**

- A. To perform comprehensive end-to-end functional testing of all features.
- B. To check the basic health and availability of the newly deployed application or service.
- C. To run security vulnerability scans on the deployed application.
- D. To gather detailed performance metrics under simulated heavy load.
- E. To verify the configuration stored in the Git repository.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**How does GitOps handle failed deployments or rollbacks compared to traditional methods?**

- A. Rollbacks require complex manual intervention on the cluster.
- B. Failures are ignored until the next successful Git commit.
- C. Rollbacks are typically achieved by reverting the change in Git and letting the operator synchronize the cluster to the previous known good state.
- D. Failed deployments automatically trigger a full cluster rebuild.
- E. Rollbacks are not possible within a GitOps framework.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is the relationship between Continuous Integration (CI) and GitOps?**

- A. GitOps replaces the need for a CI server entirely.
- B. CI builds artifacts (e.g., container images); GitOps often consumes these artifacts for deployment based on Git state.
- C. CI is responsible for deploying manifests; GitOps is responsible for building images.
- D. They are mutually exclusive approaches to application delivery.
- E. GitOps is a specific tool used only within CI pipelines.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**Which cloud-native principle supports the idea of automating infrastructure provisioning alongside application deployment?**

- A. Infrastructure as Code (IaC)
- B. Manual server configuration
- C. Stateful application design
- D. High latency tolerance.
- E. Reactive programming

<details><summary>Answer</summary>

**Correct answer:** A

</details>

---

**In a pull-based GitOps model, how does the operator typically authenticate to the Git repository?**

- A. Using the developer's personal Git credentials stored in a Secret.
- B. Using SSH keys, deploy tokens, or access tokens configured specifically for the operator.
- C. No authentication is required if the repository is public.
- D. Using Kubernetes ServiceAccount tokens intended for API server access.
- E. Authentication is handled by the CI server, not the operator.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**What does a "release candidate" (RC) typically signify in a software release process?**

- A. The final, generally available (GA) version of the software.
- B. An unstable nightly build intended only for internal testing.
- C. A version believed to be stable and potentially the final release, undergoing final testing.
- D. A prototype version demonstrating initial concepts.
- E. A security patch applied to a previous release.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is a key benefit of decoupling application configuration from container images?**

- A. It simplifies the container build process by including configuration directly.
- B. It allows the same container image to be deployed across different environments with varying configurations.
- C. It eliminates the need for version control for configuration.
- D. It makes container images larger and slower to pull.
- E. It prevents the use of Kubernetes ConfigMaps and Secrets.

<details><summary>Answer</summary>

**Correct answer:** B

</details>

---

**How does GitOps facilitate collaboration between development and operations teams?**

- A. By requiring operations teams to manually approve every developer commit.
- B. By providing separate Git repositories for developers and operators with no overlap.
- C. By using a shared Git repository and pull requests as a common mechanism for proposing and reviewing infrastructure and application changes.
- D. By eliminating the need for an operations team entirely.
- E. By forcing developers to manage the underlying Kubernetes infrastructure.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What is the role of Helm in a GitOps workflow?**

- A. Helm replaces the Git repository as the source of truth.
- B. Helm is the GitOps operator that reconciles the cluster state.
- C. Helm charts (stored in Git) can declaratively define the application, and GitOps tools deploy/manage Helm releases based on Git state.
- D. Helm is used only for building container images within the CI pipeline.
- E. Helm directly monitors application performance and triggers rollbacks.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---

**What does the "convergence" mean in the context of a GitOps reconciliation loop?**

- A. The process of merging multiple Git branches into one.
- B. The act of manually applying configuration changes to the cluster.
- C. The process where the GitOps operator brings the actual cluster state into alignment with the desired state defined in Git.
- D. The final stage of a CI pipeline where tests are run.
- E. The point where application performance meets SLO targets.

<details><summary>Answer</summary>

**Correct answer:** C

</details>

---
