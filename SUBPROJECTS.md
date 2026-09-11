# Microcks Project and Repository Inventory

This document is the canonical inventory of public, first-party repositories owned by the [Microcks GitHub organization](https://github.com/microcks). It records repository purpose, lifecycle status and responsible ownership without treating external forks, private repositories or every repository as a governed subproject.

Last reviewed: 2026-09-09

## Scope and ownership

The inventory includes public repositories owned by Microcks that are not forks. External forks and private repositories are excluded. Archived first-party repositories remain listed so that their status and history stay visible.

The [central Maintainers and Code Owners list](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) is authoritative for project governance roles. A repository `CODEOWNERS` file identifies the people automatically requested to review changes in that repository; it does not grant a project governance role by itself. When no repository-specific ownership record exists, the top-level Maintainers are responsible.

Changes to repository lifecycle or ownership must update this inventory in the same decision or pull request. The Maintainers review the inventory at least annually.

## External project health checks

CNCF [CLOMonitor](https://clomonitor.io/projects/cncf/microcks) evaluates selected Microcks repositories using the repository-specific check sets declared in the [CNCF CLOMonitor configuration](https://github.com/cncf/clomonitor/blob/main/data/cncf.yaml).

CLOMonitor provides an external project health and conformance signal. This inventory remains authoritative for Microcks repository scope, lifecycle and ownership. A repository not configured in CLOMonitor is not necessarily unsupported or excluded from the project.

## Categories

- **Core product:** The main Microcks application and its primary delivery components.
- **Integration:** An extension or adapter connecting Microcks to another platform or developer workflow.
- **SDK or library:** A reusable client, runtime or testing library.
- **Tooling:** Automation, packaging or utilities supporting Microcks users and contributors.
- **Demonstration or workshop:** Educational examples and hands-on learning material; these are not production deliverables.
- **Website or content:** Documentation, websites, catalogs and reusable content.
- **Community or governance:** Project-wide governance, community coordination and CNCF metadata.
- **Infrastructure:** Images or other assets used to build and operate Microcks services.

## Lifecycle states

- **Experimental:** Exploratory work for which compatibility and long-term support are not yet promised.
- **Active:** Supported work that may receive features, fixes, releases or content updates.
- **Maintenance:** Supported work limited primarily to security and critical fixes.
- **Deprecated:** Work with a documented replacement or migration path that is preparing for archival.
- **Archived:** Read-only historical work that no longer receives fixes or releases.

A lifecycle change requires the formal decision process defined in [GOVERNANCE.md](https://github.com/microcks/.github/blob/main/GOVERNANCE.md#decision-making-and-voting). Before a repository becomes Deprecated, its documentation should identify any replacement and migration path. Archived repositories remain in this inventory. Any future transfer to a dedicated archive organization must be approved as a repository removal and recorded here, with redirects or successor links where practical.

## Active repositories

| Repository | Category | Purpose | Lifecycle | Responsible owners | Ownership record |
| --- | --- | --- | --- | --- | --- |
| [microcks](https://github.com/microcks/microcks) | Core product | API mocking and testing platform | Active | [@lbroudoux](https://github.com/lbroudoux), [@yada](https://github.com/yada), [@SebastienDegodez](https://github.com/SebastienDegodez) | [CODEOWNERS](https://github.com/microcks/microcks/blob/master/CODEOWNERS) |
| [microcks-operator](https://github.com/microcks/microcks-operator) | Core product | Kubernetes Operator for deploying and managing Microcks | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-cli](https://github.com/microcks/microcks-cli) | Tooling | Command-line client for Microcks APIs | Active | [@lbroudoux](https://github.com/lbroudoux), [@yada](https://github.com/yada), [@Harsh4902](https://github.com/Harsh4902) | [CODEOWNERS](https://github.com/microcks/microcks-cli/blob/master/CODEOWNERS) |
| [microcks-mcp-server](https://github.com/microcks/microcks-mcp-server) | Integration | MCP server for interacting with Microcks from agents and MCP clients | Active | [@lbroudoux](https://github.com/lbroudoux), [@yada](https://github.com/yada) | [CODEOWNERS](https://github.com/microcks/microcks-mcp-server/blob/main/CODEOWNERS) |
| [microcks-agent-skills](https://github.com/microcks/microcks-agent-skills) | Tooling | Agent skills and integrations for Microcks workflows | Active | [@lbroudoux](https://github.com/lbroudoux), [@yada](https://github.com/yada), [@SebastienDegodez](https://github.com/SebastienDegodez) | [CODEOWNERS](https://github.com/microcks/microcks-agent-skills/blob/main/CODEOWNERS) |
| [microcks-postman-runtime](https://github.com/microcks/microcks-postman-runtime) | SDK or library | HTTP bridge for executing Postman tests | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-postman-runtime/blob/master/CODEOWNERS) |
| [microcks-testcontainers-java](https://github.com/microcks/microcks-testcontainers-java) | SDK or library | Java Testcontainers integration | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-testcontainers-java/blob/main/CODEOWNERS) |
| [microcks-testcontainers-go](https://github.com/microcks/microcks-testcontainers-go) | SDK or library | Go Testcontainers integration | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-testcontainers-go/blob/main/CODEOWNERS) |
| [microcks-testcontainers-node](https://github.com/microcks/microcks-testcontainers-node) | SDK or library | Node.js and TypeScript Testcontainers integration | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-testcontainers-node/blob/main/CODEOWNERS) |
| [microcks-testcontainers-dotnet](https://github.com/microcks/microcks-testcontainers-dotnet) | SDK or library | .NET Testcontainers integration | Active | [@SebastienDegodez](https://github.com/SebastienDegodez), [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-testcontainers-dotnet/blob/main/CODEOWNERS) |
| [microcks-quarkus](https://github.com/microcks/microcks-quarkus) | Integration | Quarkus extension for Microcks Dev Services and contract testing | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-quarkus/blob/main/CODEOWNERS) |
| [microcks-aspire](https://github.com/microcks/microcks-aspire) | Integration | .NET Aspire integration for hosting and testing with Microcks | Active | [@SebastienDegodez](https://github.com/SebastienDegodez), [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-aspire/blob/main/CODEOWNERS) |
| [microcks-java-client](https://github.com/microcks/microcks-java-client) | SDK or library | Java client for the Microcks API | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-go-client](https://github.com/microcks/microcks-go-client) | SDK or library | Go client for the Microcks API | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-go-client/blob/main/CODEOWNERS) |
| [microcks-docker-desktop-extension](https://github.com/microcks/microcks-docker-desktop-extension) | Integration | Docker Desktop extension for running Microcks | Active | [@lbroudoux](https://github.com/lbroudoux), [@hguerrero](https://github.com/hguerrero) | [CODEOWNERS](https://github.com/microcks/microcks-docker-desktop-extension/blob/main/CODEOWNERS) |
| [microcks-backstage-provider](https://github.com/microcks/microcks-backstage-provider) | Integration | Backstage provider for synchronizing API entities from Microcks | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-jenkins-plugin](https://github.com/microcks/microcks-jenkins-plugin) | Integration | Jenkins plugin for running Microcks tests | Active | [@lbroudoux](https://github.com/lbroudoux), [@yada](https://github.com/yada) | [CODEOWNERS](https://github.com/microcks/microcks-jenkins-plugin/blob/master/CODEOWNERS) |
| [microcks-spectral-ruleset](https://github.com/microcks/microcks-spectral-ruleset) | Tooling | Spectral rules for Microcks OpenAPI and AsyncAPI conventions | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-spectral-ruleset/blob/main/CODEOWNERS) |
| [import-github-action](https://github.com/microcks/import-github-action) | Tooling | GitHub Action for importing API specifications into Microcks | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/import-github-action/blob/main/CODEOWNERS) |
| [test-github-action](https://github.com/microcks/test-github-action) | Tooling | GitHub Action for running Microcks tests | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/test-github-action/blob/main/CODEOWNERS) |
| [homebrew-tap](https://github.com/microcks/homebrew-tap) | Tooling | Homebrew formulae for Microcks tools | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [api-tooling](https://github.com/microcks/api-tooling) | Tooling | API development, testing, validation and migration utilities | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [hub.microcks.io](https://github.com/microcks/hub.microcks.io) | Website or content | Public catalog for reusable Microcks mocks and tests | Active | [@lbroudoux](https://github.com/lbroudoux), [@yada](https://github.com/yada) | [CODEOWNERS](https://github.com/microcks/hub.microcks.io/blob/master/CODEOWNERS) |
| [community-mocks](https://github.com/microcks/community-mocks) | Website or content | Community mocks and tests published through the Microcks Hub | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-quickstarters](https://github.com/microcks/microcks-quickstarters) | Website or content | Reusable API examples for industry and vertical standards | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-images](https://github.com/microcks/microcks-images) | Infrastructure | Base container images used by Microcks | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-testcontainers-java-spring-demo](https://github.com/microcks/microcks-testcontainers-java-spring-demo) | Demonstration or workshop | Spring Boot example using Microcks Testcontainers | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-quarkus-demo](https://github.com/microcks/microcks-quarkus-demo) | Demonstration or workshop | Quarkus example using Microcks Dev Services and Testcontainers | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-testcontainers-node-nest-demo](https://github.com/microcks/microcks-testcontainers-node-nest-demo) | Demonstration or workshop | NestJS example using Microcks Testcontainers | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-testcontainers-node-nest-demo/blob/main/CODEOWNERS) |
| [microcks-testcontainers-go-demo](https://github.com/microcks/microcks-testcontainers-go-demo) | Demonstration or workshop | Go example using Microcks Testcontainers | Active | [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-testcontainers-go-demo/blob/main/CODEOWNERS) |
| [microcks-testcontainers-dotnet-demo](https://github.com/microcks/microcks-testcontainers-dotnet-demo) | Demonstration or workshop | .NET example using Microcks Testcontainers | Active | [@SebastienDegodez](https://github.com/SebastienDegodez), [@lbroudoux](https://github.com/lbroudoux) | [CODEOWNERS](https://github.com/microcks/microcks-testcontainers-dotnet-demo/blob/main/CODEOWNERS) |
| [microcks-aspire-demo](https://github.com/microcks/microcks-aspire-demo) | Demonstration or workshop | .NET Aspire example using the Microcks Aspire integration | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [api-lifecycle](https://github.com/microcks/api-lifecycle) | Demonstration or workshop | End-to-end API lifecycle demonstration | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-testcontainers-java-workshop](https://github.com/microcks/microcks-testcontainers-java-workshop) | Demonstration or workshop | Workshop for the Java Testcontainers integration | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-quarkus-workshop](https://github.com/microcks/microcks-quarkus-workshop) | Demonstration or workshop | Workshop for Microcks Quarkus Dev Services | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks-testcontainers-dotnet-workshop](https://github.com/microcks/microcks-testcontainers-dotnet-workshop) | Demonstration or workshop | Workshop for the .NET Testcontainers integration | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks.io](https://github.com/microcks/microcks.io) | Website or content | Microcks website and documentation source | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [microcks.github.io](https://github.com/microcks/microcks.github.io) | Website or content | Published Microcks website content | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [.github](https://github.com/microcks/.github) | Community or governance | Canonical organization governance and community health files | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [community](https://github.com/microcks/community) | Community or governance | Community meetings, steering material and collaborative resources | Active | Top-level Maintainers | [Central MAINTAINERS](https://github.com/microcks/.github/blob/main/MAINTAINERS.md) |
| [.project](https://github.com/microcks/.project) | Community or governance | CNCF project metadata and automation | Active | Project Maintainers and Steering Committee | [CODEOWNERS](https://github.com/microcks/.project/blob/main/CODEOWNERS) |

## Archived repositories

| Repository | Category | Purpose | Lifecycle | Responsible owners | Ownership record |
| --- | --- | --- | --- | --- | --- |
| [microcks-ansible-operator](https://github.com/microcks/microcks-ansible-operator) | Core product | Former Ansible-based Kubernetes Operator | Archived | Top-level Maintainers for archive stewardship | [CODEOWNERS](https://github.com/microcks/microcks-ansible-operator/blob/master/CODEOWNERS) |
| [microcks-go-operator](https://github.com/microcks/microcks-go-operator) | Core product | Former Go-based Kubernetes Operator | Archived | Top-level Maintainers for archive stewardship | No repository-specific ownership record |
| [microcks-keycloak](https://github.com/microcks/microcks-keycloak) | Infrastructure | Former Microcks Keycloak distribution | Archived | Top-level Maintainers for archive stewardship | No repository-specific ownership record |
| [microcks-azure](https://github.com/microcks/microcks-azure) | Tooling | Former Azure deployment templates and scripts | Archived | Top-level Maintainers for archive stewardship | No repository-specific ownership record |

## Deliberate exclusions

The following repositories are not entries in this first-party inventory:

- **External forks:** `agent-bond`, `backstage`, `community-module-registry`, `community-operators`, `community-operators-1`, `community-operators-prod`, `graphql.github.io`, `hub`, `java`, `microk8s-community-addons`, `protoc-jar`, `quarkus-extension-catalog` and `website`.
- **Private repositories:** Private repositories are excluded from this public inventory and are not enumerated here.

This inventory does not control distribution of organization-level files. Those files are replicated to the repositories where they are needed and relevant according to the deliberate per-file scope and exclusions in the [replication workflow](https://github.com/microcks/.github/blob/main/.github/workflows/global-replicator.yml).
