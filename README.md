# Platform Capstone

A hands-on DevOps platform project built step by step, with every stage documented so it can be reproduced from scratch.

## Goal

Build a production-style platform that takes an application from code commit to a running deployment, with automated builds, GitOps delivery, and monitoring.

## Architecture

Code -> CI pipeline -> Container registry -> Kubernetes cluster -> Monitoring

## Tech Stack

| Area | Tools |
|---|---|
| Cloud | AWS |
| Containers and orchestration | Docker, Kubernetes |
| CI/CD | Jenkins or GitHub Actions |
| GitOps | ArgoCD |
| Infrastructure as Code | Terraform |
| Observability | Prometheus, Grafana |

## Repository Structure

| Folder | Purpose |
|---|---|
| `app/` | The application source code and its Dockerfile. |
| `docs/` | Architecture diagrams, screenshots, and project documentation. |
| `k8s/` | Kubernetes manifests (or Helm charts) that deploy the application to the cluster. |
| `notes/` | Daily learning notes and the problems I hit and fixed. |
| `observability/` | Prometheus and Grafana configuration, dashboards, and alert rules. |
| `runbooks/` | Step-by-step guides for handling incidents, such as what to do when a pod crashes or the site is down. |
| `terraform/` | Infrastructure as Code that creates the cloud resources, such as the network and the cluster. |

## Progress

- [x] Repo and folder structure set up
- [x] Application source code added to the repo
- [ ] Infrastructure created with Terraform
- [ ] CI pipeline builds and pushes the image
- [ ] Application deployed to Kubernetes
- [ ] GitOps delivery set up with ArgoCD
- [ ] Monitoring and dashboards set up with Prometheus and Grafana
- [ ] Runbooks written for common incidents
      

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/neerajramakrishna-sys/platform-capstone
   cd platform-capstone
   ```
2. Prerequisites: Git, Docker, kubectl, Terraform, and the AWS CLI.
3. Follow the README inside each folder, in the order shown in the Progress list.

## Learning Log

Short notes on problems hit and how they were fixed.

| Date | Problem | Fix |
|---|---|---|
| 2026-10-16 | Folders created locally did not show on GitHub | Git does not track empty folders, so I added a `.gitkeep` file to each one and pushed. |


## Author

Neeraj - building towards a DevOps career.
Application source code is from Docker's example voting app. All Dockerfiles, compose files, Kubernetes manifests, and infrastructure in this repository were written by me.
