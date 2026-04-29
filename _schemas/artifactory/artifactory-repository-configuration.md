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
source_filename: artifactory-repository-configuration.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/artifactory-repository-configuration.json\",\n  \"title\": \"Artifactory Repository Configuration\",\n  \"description\": \"Configuration schema for JFrog Artifactory repositories including local, remote, virtual, and federated types.\",\n  \"type\": \"object\",\n  \"required\": [\"key\", \"rclass\"],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique repository identifier. Must be lowercase and can contain letters, digits, hyphens, dots, and underscores.\",\n      \"pattern\": \"^[a-zA-Z0-9][a-zA-Z0-9._-]*$\",\n      \"examples\": [\"libs-release-local\", \"npm-remote\", \"docker-virtual\"]\n    },\n    \"rclass\": {\n      \"type\": \"string\",\n      \"description\": \"Repository class that determines repository behavior.\",\n      \"enum\": [\"local\", \"remote\", \"virtual\", \"federated\"]\n    },\n    \"packageType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The package type this repository handles.\",\n      \"enum\": [\n        \"maven\",\n        \"gradle\",\n        \"ivy\",\n        \"sbt\",\n        \"helm\",\n        \"cocoapods\",\n        \"opkg\",\n        \"rpm\",\n        \"nuget\",\n        \"cran\",\n        \"gems\",\n        \"npm\",\n        \"bower\",\n        \"debian\",\n        \"composer\",\n        \"pypi\",\n        \"docker\",\n        \"vagrant\",\n        \"gitlfs\",\n        \"go\",\n        \"conan\",\n        \"chef\",\n        \"puppet\",\n        \"generic\",\n        \"cargo\",\n        \"conda\",\n        \"swift\",\n        \"terraform\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the repository.\",\n      \"maxLength\": 1024\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Internal notes about the repository (not visible to end users).\"\
  ,\n      \"maxLength\": 1024\n    },\n    \"includesPattern\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of artifact path patterns to include.\",\n      \"default\": \"**/*\"\n    },\n    \"excludesPattern\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of artifact path patterns to exclude.\",\n      \"default\": \"\"\n    },\n    \"repoLayoutRef\": {\n      \"type\": \"string\",\n      \"description\": \"Repository layout reference name.\",\n      \"examples\": [\"maven-2-default\", \"npm-default\", \"simple-default\"]\n    },\n    \"handleReleases\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this repository handles release artifacts.\",\n      \"default\": true\n    },\n    \"handleSnapshots\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this repository handles snapshot artifacts.\",\n      \"default\": false\n    },\n    \"maxUniqueSnapshots\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Maximum number of unique snapshots to retain. 0 means unlimited.\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"suppressPomConsistencyChecks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to suppress POM consistency checks for Maven artifacts.\",\n      \"default\": false\n    },\n    \"blackedOut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is blacked out (all access denied).\",\n      \"default\": false\n    },\n    \"propertySets\": {\n      \"type\": \"array\",\n      \"description\": \"List of property set names to associate with this repository.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"archiveBrowsingEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether browsing of archive contents is enabled.\",\n      \"default\": false\n    },\n    \"xrayIndex\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether JFrog\
  \ Xray indexing is enabled for this repository.\",\n      \"default\": false\n    },\n    \"environments\": {\n      \"type\": \"array\",\n      \"description\": \"List of environments this repository is associated with.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [[\"DEV\", \"PROD\"]]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the remote repository (only for remote repositories).\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username for authenticating with the remote repository.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for authenticating with the remote repository.\"\n    },\n    \"proxy\": {\n      \"type\": \"string\",\n      \"description\": \"Proxy key for remote repository connections.\"\n    },\n    \"remoteRepoChecksumPolicyType\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Checksum policy for remote repository.\",\n      \"enum\": [\n        \"generate-if-absent\",\n        \"fail\",\n        \"ignore-and-generate\",\n        \"pass-thru\"\n      ]\n    },\n    \"unusedArtifactsCleanupPeriodHours\": {\n      \"type\": \"integer\",\n      \"description\": \"Hours to keep unused artifacts before cleanup. 0 means disabled.\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"assumedOfflinePeriodSecs\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds to assume remote is offline after a failure.\",\n      \"minimum\": 0,\n      \"default\": 300\n    },\n    \"retrievalCachePeriodSecs\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds to cache retrieval results from remote.\",\n      \"minimum\": 0,\n      \"default\": 7200\n    },\n    \"missedRetrievalCachePeriodSecs\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds to cache missed retrieval attempts.\",\n      \"minimum\": 0,\n      \"default\"\
  : 1800\n    },\n    \"repositories\": {\n      \"type\": \"array\",\n      \"description\": \"List of repository keys resolved by this virtual repository.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"defaultDeploymentRepo\": {\n      \"type\": \"string\",\n      \"description\": \"Default deployment repository for virtual repository deployments.\"\n    },\n    \"dockerApiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Docker API version for Docker repositories.\",\n      \"enum\": [\"V1\", \"V2\"]\n    },\n    \"forceNugetAuthentication\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to force authentication for NuGet repositories.\",\n      \"default\": false\n    },\n    \"enableTokenAuthentication\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether token authentication is enabled for Docker repositories.\",\n      \"default\": true\n    }\n  },\n  \"allOf\": [\n    {\n      \"if\": {\n        \"\
  properties\": {\n          \"rclass\": { \"const\": \"remote\" }\n        },\n        \"required\": [\"rclass\"]\n      },\n      \"then\": {\n        \"required\": [\"url\"]\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/json-schema/artifactory-repository-configuration.json
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
