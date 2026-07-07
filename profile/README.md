# OpenGW Project

OpenGW Project is a small, public gateway-control-plane project made up of multiple repositories:

- [web-client](https://github.com/opengw-project/web-client) — the TypeScript/Vite frontend for the API gateway control plane
- [control-plane](https://github.com/opengw-project/control-plane) — the Java/Spring Boot backend that serves gateway administration APIs
- [data-plane](https://github.com/opengw-project/data-plane) — the Rust data plane/runtime component
- [root](https://github.com/opengw-project/root) — Python-based root/orchestration utilities
- [bouncer](https://github.com/opengw-project/bouncer) — Rust service likely focused on access/control concerns
- [.github-private](https://github.com/opengw-project/.github-private) — private org-level GitHub configuration repository

## What this project is about

This organization appears to be building an API gateway platform with clear control-plane/data-plane separation:

- **web-client** provides a browser-based admin UI.
- **control-plane** exposes management APIs and configuration surfaces.
- **data-plane** likely executes request handling/runtime behaviors.
- Supporting repos (**root**, **bouncer**) appear to provide internal tooling and platform services.

## Public repositories

| Repository | Description | Primary language | URL |
| --- | --- | --- | --- |
| [web-client](https://github.com/opengw-project/web-client) | Frontend for the API gateway control plane. Built with React, TypeScript, and Vite. | TypeScript | https://github.com/opengw-project/web-client |
| [control-plane](https://github.com/opengw-project/control-plane) | Spring Boot backend for the API gateway control plane. Exposes admin APIs for routes, policies, API keys, nodes, and users. | Java | https://github.com/opengw-project/control-plane |
| [.github](https://github.com/opengw-project/.github) | Organization profile and shared community/configuration files. | — | https://github.com/opengw-project/.github |

## Additional repositories (organization-wide summary)

| Repository | Visibility | Summary | Primary language | URL |
| --- | --- | --- | --- | --- |
| [.github-private](https://github.com/opengw-project/.github-private) | Private | Private organization-level GitHub settings/automation repository. | — | https://github.com/opengw-project/.github-private |
| [bouncer](https://github.com/opengw-project/bouncer) | Private | Rust service repository, likely handling platform edge access or policy enforcement concerns. | Rust | https://github.com/opengw-project/bouncer |
| [data-plane](https://github.com/opengw-project/data-plane) | Private | Rust data-plane component likely responsible for runtime gateway traffic handling. | Rust | https://github.com/opengw-project/data-plane |
| [root](https://github.com/opengw-project/root) | Private | Python repository for root-level tooling, orchestration, or project automation. | Python | https://github.com/opengw-project/root |

## Important note

This project is heavily vibecoded. Expect rapid iteration, rough edges, and code that may favor momentum over polish. Treat it as a work in progress.

## Summary

If you want to understand the system quickly:

1. Start with `control-plane` to see the backend API surface and data flow.
2. Then open `web-client` to see how the UI consumes those APIs.
3. Explore `data-plane` for runtime execution architecture.
4. Review `root` and `bouncer` for platform support and service boundaries.
5. Expect the repository layout and implementation style to evolve quickly.
