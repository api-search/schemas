---
description: Represents a repository configuration in JFrog Artifactory, defining how artifacts are stored, proxied, or aggregated from multiple sources.
layout: schema
name: JFrog Repository
properties_list:
- description: Unique identifier for the repository
  name: key
  type: string
- description: Repository class defining its behavior
  name: rclass
  type: string
- description: Type of packages stored in this repository
  name: packageType
  type: string
- description: Free-text description of the repository
  name: description
  type: string
- description: Internal notes about the repository
  name: notes
  type: string
- description: Artifact include pattern
  name: includesPattern
  type: string
- description: Artifact exclude pattern
  name: excludesPattern
  type: string
- description: Repository layout reference
  name: repoLayoutRef
  type: string
- description: Whether to handle release artifacts
  name: handleReleases
  type: boolean
- description: Whether to handle snapshot artifacts
  name: handleSnapshots
  type: boolean
- description: Maximum number of unique snapshots to retain
  name: maxUniqueSnapshots
  type: integer
- description: Whether to suppress POM consistency checks
  name: suppressPomConsistencyChecks
  type: boolean
- description: Whether the repository is blacked out (disabled)
  name: blackedOut
  type: boolean
- description: Whether the repository is indexed by Xray for scanning
  name: xrayIndex
  type: boolean
- description: Property sets associated with the repository
  name: propertySets
  type: array
- description: Docker API version (V1 or V2)
  name: dockerApiVersion
  type: string
- description: URL of the remote repository (remote repos only)
  name: url
  type: string
- description: Username for remote repository authentication
  name: username
  type: string
- description: Environments this repository is associated with
  name: environments
  type: array
- description: Project key if the repository belongs to a project
  name: projectKey
  type: string
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-repository-schema.json
slug: jfrog-repository
source_filename: jfrog-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/repository\",\n  \"title\": \"JFrog Repository\",\n  \"description\": \"Represents a repository configuration in JFrog Artifactory, defining how artifacts are stored, proxied, or aggregated from multiple sources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the repository\",\n      \"pattern\": \"^[a-zA-Z0-9][a-zA-Z0-9._-]*$\",\n      \"examples\": [\n        \"libs-release-local\",\n        \"npm-remote\",\n        \"maven-virtual\"\n      ]\n    },\n    \"rclass\": {\n      \"type\": \"string\",\n      \"description\": \"Repository class defining its behavior\",\n      \"enum\": [\n        \"local\",\n        \"remote\",\n        \"virtual\",\n        \"federated\"\n      ]\n    },\n    \"packageType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of packages\
  \ stored in this repository\",\n      \"enum\": [\n        \"maven\",\n        \"gradle\",\n        \"ivy\",\n        \"sbt\",\n        \"helm\",\n        \"cocoapods\",\n        \"opkg\",\n        \"rpm\",\n        \"nuget\",\n        \"cran\",\n        \"gems\",\n        \"npm\",\n        \"bower\",\n        \"debian\",\n        \"composer\",\n        \"pypi\",\n        \"docker\",\n        \"vagrant\",\n        \"gitlfs\",\n        \"go\",\n        \"yum\",\n        \"conan\",\n        \"chef\",\n        \"puppet\",\n        \"generic\",\n        \"conda\",\n        \"p2\",\n        \"swift\",\n        \"terraform\",\n        \"cargo\",\n        \"oci\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text description of the repository\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Internal notes about the repository\"\n    },\n    \"includesPattern\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Artifact include pattern\",\n      \"default\": \"**/*\"\n    },\n    \"excludesPattern\": {\n      \"type\": \"string\",\n      \"description\": \"Artifact exclude pattern\",\n      \"default\": \"\"\n    },\n    \"repoLayoutRef\": {\n      \"type\": \"string\",\n      \"description\": \"Repository layout reference\",\n      \"examples\": [\n        \"maven-2-default\",\n        \"npm-default\",\n        \"simple-default\"\n      ]\n    },\n    \"handleReleases\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to handle release artifacts\"\n    },\n    \"handleSnapshots\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to handle snapshot artifacts\"\n    },\n    \"maxUniqueSnapshots\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of unique snapshots to retain\",\n      \"minimum\": 0\n    },\n    \"suppressPomConsistencyChecks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to suppress POM consistency\
  \ checks\"\n    },\n    \"blackedOut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is blacked out (disabled)\"\n    },\n    \"xrayIndex\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the repository is indexed by Xray for scanning\"\n    },\n    \"propertySets\": {\n      \"type\": \"array\",\n      \"description\": \"Property sets associated with the repository\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"dockerApiVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Docker API version (V1 or V2)\",\n      \"enum\": [\n        \"V1\",\n        \"V2\"\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the remote repository (remote repos only)\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Username for remote repository authentication\"\n    },\n    \"environments\": {\n   \
  \   \"type\": \"array\",\n      \"description\": \"Environments this repository is associated with\",\n      \"items\": {\n        \"type\": \"string\",\n        \"examples\": [\n          \"DEV\",\n          \"PROD\"\n        ]\n      }\n    },\n    \"projectKey\": {\n      \"type\": \"string\",\n      \"description\": \"Project key if the repository belongs to a project\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"rclass\",\n    \"packageType\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-repository-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Repository
---
