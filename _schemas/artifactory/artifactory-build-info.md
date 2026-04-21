---
description: Schema for JFrog Artifactory build information, representing a CI/CD build record including modules, artifacts, dependencies, and environment details.
layout: schema
name: Artifactory Build Info
properties_list:
- description: Build info JSON schema version.
  name: version
  type: string
- description: Build name identifier.
  name: name
  type: string
- description: Build number (version string).
  name: number
  type: string
- description: Build type corresponding to the build tool used.
  name: type
  type: string
- description: Information about the CI server agent.
  name: agent
  type: object
- description: Information about the build tool agent.
  name: buildAgent
  type: object
- description: ISO 8601 timestamp of when the build started.
  name: started
  type: string
- description: Build duration in milliseconds.
  name: durationMillis
  type: integer
- description: The user principal who triggered the build.
  name: principal
  type: string
- description: The Artifactory user associated with the build.
  name: artifactoryPrincipal
  type: string
- description: URL to the build in the CI server.
  name: url
  type: string
- description: VCS revision (e.g., Git commit SHA).
  name: vcsRevision
  type: string
- description: VCS repository URL.
  name: vcsUrl
  type: string
- description: Detailed VCS information for multi-module builds.
  name: vcs
  type: array
- description: Build modules, each representing a logical unit of the build.
  name: modules
  type: array
- description: Build promotion status history.
  name: statuses
  type: array
- description: Build-level custom properties.
  name: properties
  type: object
- description: Other builds this build depends on.
  name: buildDependencies
  type: array
provider_name: JFrog Artifactory
provider_slug: artifactory
schema_file: json-schema/artifactory-build-info.json
slug: artifactory-build-info
tags:
- Artifacts
- DevOps
- CI/CD
- Docker Registry
- Maven
- Package Management
- Repository
title: Artifactory Build Info
---
