# Google Summer of Code 2023 - Project Showcase

## Project: Improved Backend Performance and Security - Talawa API

- [Project Overview](#project-overview)
- [Project Milestones](#project-milestones)
  - [1. GraphQL Inspector for API Versioning](#1-graphql-inspector-for-api-versioning)
  - [2. Apollo Server Migration](#2-apollo-server-migration)
  - [3. GraphQL Error-Handling](#3-graphql-error-handling)
  - [4. Caching Entities using Redis](#4-caching-entities-using-redis)
  - [5. Access Control Enforcement in Resolvers](#5-access-control-enforcement-in-resolvers)
  - [6. Encryption of PII Data](#6-encryption-of-pii-data)
  - [7. HTTPS Configuration](#7-https-configuration)
  - [8. Encryption Helpers](#8-encryption-helpers)
- [Impact and Future Work](#impact-and-future-work)
- [References](#references)


This markdown document highlights the key accomplishments and contributions made during my participation in Google Summer of Code 2023 for the Palisadoes Foundation and the Talawa GraphQL API project. 

### Project Overview

The primary goal of this project was to enhance the Talawa GraphQL API by addressing various issues and improving its overall performance and security.

### Project Milestones

#### 1. GraphQL Inspector for API Versioning

- ([PR-Link](https://github.com/PalisadoesFoundation/talawa-api/pull/1340))
- Monitored 100% of API schema using GraphQL-Inspector, ensuring seamless communication of schema
updates to client apps
- Implemented versioning in local machine and CI/CD pipeline for each commit in a
Pull Request (Github Actions), resulting in improved development efficiency and reduced API compatibility
issues.
- Implemented GraphQL Inspector for efficient API versioning, 
- Impact: Improving the maintainability and scalability of the API.

#### 2. Apollo Server Migration
- ([PR-Link](https://github.com/PalisadoesFoundation/talawa-api/pull/1351))
- Migrated the deprecated Apollo server v2.0 to a newer LTS v4 .
- Ensured that the API's dependencies are up-to-date and more secure.

#### 3. GraphQL Error-Handling

- ([PR-Link](https://github.com/PalisadoesFoundation/talawa-docs/pull/593))
- Conducted documentation for GraphQL error-handling mechanisms.
- Delayed implementation due to breaking changes, prioritized for post-GSoC period.

#### 4. Caching Entities using Redis

- ([PR-Link-1](https://github.com/PalisadoesFoundation/talawa-api/pull/1377))
- ([PR-Link-2](https://github.com/PalisadoesFoundation/talawa-api/pull/1388))
- Implemented caching of database entries using Redis.
- Optimized data retrieval by implementing Redis as an in-memory cache; using table denormalization to reduce
API query process time from 12.5ms to 0.5ms during cache hit, resulting in a remarkable 99.6% improvement
by reducing database query overhead

#### 5. Access Control Enforcement in Resolvers

- ([PR-Link](https://github.com/PalisadoesFoundation/talawa-api/pull/1073))
- Resolved business logic bugs and enhanced security by enforcing access control.
- Ensured features adhere to defined constraints.
- Details: [Talawa API Constraints](https://docs.talawa.io/docs/developers/talawa-api/constraints/admin)

#### 6. Encryption of PII Data

- ([PR-Link for next 3 milestones](https://github.com/PalisadoesFoundation/talawa-api/pull/1407))
- Enhanced security by encrypting Personally Identifiable Information (PII) data stored on disk.
- Improved security with encryption within the SSL layer.

#### 7. HTTPS Configuration

- Configured HTTPS for the production environment, enhancing overall security.

#### 8. Encryption Helpers

- Merged encryption helpers into the project.
- Continued exploring and refining logic according to business requirements and access control.

### Impact and Future Work

The work done during Google Summer of Code significantly improved the Talawa GraphQL API's performance and security. Notable accomplishments include versioning, server migration, caching, access control, and configuration of HTTPS.

This project lays the foundation for a more secure and efficient Talawa API, and there are ongoing discussions and refinements to ensure its continued success.

For further details and in-depth discussions, you can refer to the project's GitHub discussions and issues.

### References

- [GitHub Discussions and Issues](https://github.com/PalisadoesFoundation/talawa-api/discussions/1239#discussioncomment-5486951)

---

**Note:** This is a high-level summary of the work completed during the GSoC project. For more detailed information and code contributions, please refer to the project's GitHub repository and related discussions.
