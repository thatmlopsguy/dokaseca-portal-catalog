# Doka Seca Portal Catalog

<div align="center">

<img src="https://raw.githubusercontent.com/thatmlopsguy/dokaseca-control-plane/main/docs/assets/logos/banner.svg" alt="DoKa Seca - Kubernetes Platform Engineering Framework" width="600"/>

</div>

<div align="center">

*Just as ships are built in dry docks, platforms are crafted in DoKa Seca*

</div>

<div align="center">
  <a href="https://github.com/thatmlopsguy/dokaseca-portal-catalog"><img src="https://img.shields.io/github/stars/thatmlopsguy/dokaseca-portal-catalog?style=flat&label=GitHub%20%E2%AD%90" alt="GitHub"></a>
  <a href="https://github.com/thatmlopsguy/dokaseca-portal-catalog/commits/main"><img src="https://img.shields.io/github/last-commit/thatmlopsguy/dokaseca-portal-catalog.svg" alt="GitHub last commit"></a>
  <a href="https://github.com/thatmlopsguy/dokaseca-portal-catalog/graphs/commit-activity"><img src="https://img.shields.io/github/commit-activity/w/thatmlopsguy/dokaseca-portal-catalog" alt="Commit activity"></a>
  <a href="https://github.com/thatmlopsguy/dokaseca-portal-catalog/issues"><img src="https://img.shields.io/github/issues/thatmlopsguy/dokaseca-portal-catalog.svg" alt="GitHub issues"></a>
  <a href="https://github.com/thatmlopsguy/dokaseca-portal-catalog/pulls"><img src="https://img.shields.io/github/issues-pr/thatmlopsguy/dokaseca-portal-catalog" alt="GitHub PRs"></a>
  <a href="https://github.com/thatmlopsguy/dokaseca-portal-catalog/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg" alt="License"></a>
  <a href="https://thatmlopsguy.github.io/dokaseca-control-plane/"><img src="https://img.shields.io/website-up-down-green-red/http/shields.io.svg" alt="Website"></a>
</div>

>⚠️ Note
>
> DoKa Seca is still in relatively early development. At this time, **do not use** Doka Seca for critical production systems.

## 👋 Introduction

Welcome to **DoKa Seca** - Distributed Orchestration Kubernetes Automation with Scalable Edge Computing Applications - a comprehensive framework for bootstrapping cloud-native platforms using Kubernetes in Docker (Kind)!

The name "DoKa Seca" is a playful Portuguese phrase where "DoKa" incorporates the "K" from Kubernetes (representing the containerized orchestration at the heart of this project), and "Seca" means "dry" - drawing inspiration from the concept of a **dry dock**. Just as ships are built, repaired, and maintained in dry docks - controlled, isolated environments where all the necessary infrastructure and tooling are readily available - DoKa Seca provides a "dry dock" for Kubernetes platforms. It creates an isolated, controlled environment where entire cloud-native platforms can be rapidly assembled, configured, and tested before being deployed to production waters.

DoKa Seca provides an opinionated, production-ready framework that automates the entire platform bootstrap process using Kind clusters. Rather than just being a collection of configurations, it's a complete platform engineering solution that provisions infrastructure, installs essential tooling, configures GitOps workflows, and sets up observability - all with a single command, in your local "dry dock" environment.

This project serves as both a personal learning journey into modern DevOps practices and a comprehensive resource for platform engineers and developers interested in rapidly spinning up production-grade Kubernetes environments. Here you'll find real-world implementations of GitOps workflows, infrastructure as code, observability stacks, and cloud-native security practices - all designed to run efficiently in local development or homelab environments while following enterprise-grade patterns and best practices.

DoKa Seca consists of 5 GitHub repositories:

| Repository                                                                         | Description                                         |
|------------------------------------------------------------------------------------|-----------------------------------------------------|
| [dokaseca-control-plane](https://github.com/thatmlopsguy/dokaseca-control-plane)   | Control plane infrastructure and cluster management |
| [dokaseca-addons](https://github.com/thatmlopsguy/dokaseca-addons)                 | Platform addons and Kubernetes extensions           |
| [dokaseca-workloads](https://github.com/thatmlopsguy/dokaseca-workloads)           | Application workloads and deployments               |
| [dokaseca-portal](https://github.com/thatmlopsguy/dokaseca-portal)                 | Backstage project (TBD) (optional)                  |
| [dokaseca-portal-catalog](https://github.com/thatmlopsguy/dokaseca-portal-catalog) | Backstage Catalog (TBD) (optional)                  |

This repository contains the catalog entities for Doka Seca's Backstage developer portal.

## Structure

```sh
catalog/
├── all.yaml              # Root location file (Backstage entry point)
├── domains/              # Business domain definitions
├── systems/              # System definitions
├── components/           # Service/component definitions
├── resources/            # Infrastructure resource definitions
└── templates/            # Golden path templates
```

## Usage

This repository is automatically read by Backstage using the GitHub integration.
Changes pushed to this repo will be discovered by Backstage within a few minutes.

## Adding New Entities

1. Create YAML files in the appropriate subdirectory
2. Add a reference to the new file in `catalog/all.yaml`
3. Push changes to GitHub
4. Wait for Backstage to discover the new entities (usually 1-5 minutes)
