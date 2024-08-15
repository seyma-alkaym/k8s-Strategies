# k8s-Strategies

This repository contains illustrative examples of three common application deployment strategies using Kubernetes: **Green-Blue Deployment**, **Canary Deployment**, and **A/B Testing**. You will find YAML files that demonstrate how to set up each strategy.

## Deployment Strategies

### 1. [Green-Blue Deployment](Green-BlueDeployment)

**Objective**: Minimize deployment time and reduce the risks associated with new application versions.

**Description**:
In the Green-Blue Deployment strategy, two versions of the application (an old "Blue" version and a new "Green" version) are run simultaneously. After testing the new version, all traffic is switched to it, while the old version remains ready for rollback if needed.

### 2. [Canary Deployment](canary)

**Objective**: Enable a gradual application update, reducing risks by testing the new version with a small portion of users before a full rollout.

**Description**:
In the Canary Deployment strategy, the new version of the application is deployed alongside the current version. A small portion of traffic is routed to the new version to monitor its performance. If no issues arise, the percentage of traffic to the new version is gradually increased until full traffic is directed to it.

### 3. [A/B Testing](A-B_Testing)

**Objective**: Test two different versions of an application to determine which one performs better or receives higher user approval.

**Description**:
In the A/B Testing strategy, two different versions of the application (A and B) are deployed. A portion of traffic is routed to each version to compare performance and user acceptance. Based on the results, a decision can be made on which version to use permanently.

## How to Use

1. **Apply the Strategies**: Deploy the appropriate YAML files to your Kubernetes environment.
2. **Customize the Settings**: Ensure you update the application names, services, and ports to match your requirements.
3. **Monitor Performance**: Use suitable monitoring tools to track the application's performance and ensure the strategy is working as expected.

## Contributing

If you would like to contribute to improving this repository or have any questions, feel free to open an issue or submit a pull request.
