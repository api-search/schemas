---
description: Schema for artifact file information returned by the Artifactory storage API, including metadata, checksums, and download URI.
layout: schema
name: Artifactory File Info
properties_list:
- description: Repository key where the file is stored.
  name: repo
  type: string
- description: Path to the file within the repository.
  name: path
  type: string
- description: ISO 8601 timestamp when the file was first created.
  name: created
  type: string
- description: Username of the user who created/deployed the file.
  name: createdBy
  type: string
- description: ISO 8601 timestamp of the last modification.
  name: lastModified
  type: string
- description: Username of the user who last modified the file.
  name: modifiedBy
  type: string
- description: ISO 8601 timestamp of the last update (including metadata changes).
  name: lastUpdated
  type: string
- description: Direct download URI for the artifact.
  name: downloadUri
  type: string
- description: Remote URL if this is a cached remote artifact.
  name: remoteUrl
  type: string
- description: MIME type of the file.
  name: mimeType
  type: string
- description: File size in bytes. May be returned as a string or integer.
  name: size
  type:
  - string
  - integer
- description: Checksums computed by Artifactory.
  name: checksums
  type: object
- description: Checksums as provided during deployment (before Artifactory verification).
  name: originalChecksums
  type: object
- description: API URI for this file info resource.
  name: uri
  type: string
provider_name: JFrog Artifactory
provider_slug: artifactory
schema_file: json-schema/artifactory-file-info.json
slug: artifactory-file-info
tags:
- Artifacts
- DevOps
- CI/CD
- Docker Registry
- Maven
- Package Management
- Repository
title: Artifactory File Info
---
