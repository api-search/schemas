---
description: Configuration schema for JFrog Artifactory repositories including local, remote, virtual, and federated types.
layout: schema
name: Artifactory Repository Configuration
properties_list:
- description: Unique repository identifier. Must be lowercase and can contain letters, digits, hyphens, dots, and underscores.
  name: key
  type: string
- description: Repository class that determines repository behavior.
  name: rclass
  type: string
- description: The package type this repository handles.
  name: packageType
  type: string
- description: Human-readable description of the repository.
  name: description
  type: string
- description: Internal notes about the repository (not visible to end users).
  name: notes
  type: string
- description: Comma-separated list of artifact path patterns to include.
  name: includesPattern
  type: string
- description: Comma-separated list of artifact path patterns to exclude.
  name: excludesPattern
  type: string
- description: Repository layout reference name.
  name: repoLayoutRef
  type: string
- description: Whether this repository handles release artifacts.
  name: handleReleases
  type: boolean
- description: Whether this repository handles snapshot artifacts.
  name: handleSnapshots
  type: boolean
- description: Maximum number of unique snapshots to retain. 0 means unlimited.
  name: maxUniqueSnapshots
  type: integer
- description: Whether to suppress POM consistency checks for Maven artifacts.
  name: suppressPomConsistencyChecks
  type: boolean
- description: Whether the repository is blacked out (all access denied).
  name: blackedOut
  type: boolean
- description: List of property set names to associate with this repository.
  name: propertySets
  type: array
- description: Whether browsing of archive contents is enabled.
  name: archiveBrowsingEnabled
  type: boolean
- description: Whether JFrog Xray indexing is enabled for this repository.
  name: xrayIndex
  type: boolean
- description: List of environments this repository is associated with.
  name: environments
  type: array
- description: URL of the remote repository (only for remote repositories).
  name: url
  type: string
- description: Username for authenticating with the remote repository.
  name: username
  type: string
- description: Password for authenticating with the remote repository.
  name: password
  type: string
- description: Proxy key for remote repository connections.
  name: proxy
  type: string
- description: Checksum policy for remote repository.
  name: remoteRepoChecksumPolicyType
  type: string
- description: Hours to keep unused artifacts before cleanup. 0 means disabled.
  name: unusedArtifactsCleanupPeriodHours
  type: integer
- description: Seconds to assume remote is offline after a failure.
  name: assumedOfflinePeriodSecs
  type: integer
- description: Seconds to cache retrieval results from remote.
  name: retrievalCachePeriodSecs
  type: integer
- description: Seconds to cache missed retrieval attempts.
  name: missedRetrievalCachePeriodSecs
  type: integer
- description: List of repository keys resolved by this virtual repository.
  name: repositories
  type: array
- description: Default deployment repository for virtual repository deployments.
  name: defaultDeploymentRepo
  type: string
- description: Docker API version for Docker repositories.
  name: dockerApiVersion
  type: string
- description: Whether to force authentication for NuGet repositories.
  name: forceNugetAuthentication
  type: boolean
- description: Whether token authentication is enabled for Docker repositories.
  name: enableTokenAuthentication
  type: boolean
provider_name: JFrog Artifactory
provider_slug: artifactory
schema_file: json-schema/artifactory-repository-configuration.json
slug: artifactory-repository-configuration
tags:
- Artifacts
- DevOps
- CI/CD
- Docker Registry
- Maven
- Package Management
- Repository
title: Artifactory Repository Configuration
---
