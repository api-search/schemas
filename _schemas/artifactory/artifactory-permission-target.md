---
description: Schema for JFrog Artifactory permission targets (V2), defining access control rules for repositories and builds. Permission targets map users and groups to specific permissions on repository and build resources.
layout: schema
name: Artifactory Permission Target
properties_list:
- description: Unique name for the permission target.
  name: name
  type: string
- description: Repository permissions section defining access to repository artifacts.
  name: repo
  type: object
- description: Build permissions section defining access to build information.
  name: build
  type: object
provider_name: JFrog Artifactory
provider_slug: artifactory
schema_file: json-schema/artifactory-permission-target.json
slug: artifactory-permission-target
tags:
- Artifacts
- DevOps
- CI/CD
- Docker Registry
- Maven
- Package Management
- Repository
title: Artifactory Permission Target
---
