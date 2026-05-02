---
description: Represents a release bundle in the JFrog Platform, which is an immutable, signed collection of artifacts that can be promoted through environments and distributed to edge nodes for reliable software delivery.
layout: schema
name: JFrog Release Bundle
properties_list:
- description: Release bundle name
  name: name
  type: string
- description: Release bundle version
  name: version
  type: string
- description: Current status of the release bundle
  name: status
  type: string
- description: Human-readable description of the release bundle
  name: description
  type: string
- description: Release notes content
  name: release_notes
  type: object
- description: Type of source used to create the release bundle
  name: source_type
  type: string
- description: Creation timestamp
  name: created
  type: string
- description: User who created the release bundle
  name: created_by
  type: string
- description: Artifacts included in the release bundle
  name: artifacts
  type: array
- description: Current promotion environment
  name: current_environment
  type: string
- description: History of environment promotions
  name: promotion_history
  type: array
- description: Distribution status to edge nodes
  name: distribution_status
  type: object
- description: Evidence and attestations attached to this release
  name: evidence
  type: array
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-release-bundle-schema.json
slug: jfrog-release-bundle
source_filename: jfrog-release-bundle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/release-bundle\",\n  \"title\": \"JFrog Release Bundle\",\n  \"description\": \"Represents a release bundle in the JFrog Platform, which is an immutable, signed collection of artifacts that can be promoted through environments and distributed to edge nodes for reliable software delivery.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Release bundle name\",\n      \"examples\": [\n        \"my-app-release\"\n      ]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Release bundle version\",\n      \"examples\": [\n        \"1.0.0\",\n        \"2025.01.15\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the release bundle\",\n      \"enum\": [\n        \"OPEN\",\n        \"SIGNED\",\n        \"STORED\",\n\
  \        \"READY_FOR_DISTRIBUTION\",\n        \"CREATED\",\n        \"PROMOTED\",\n        \"DISTRIBUTED\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the release bundle\"\n    },\n    \"release_notes\": {\n      \"type\": \"object\",\n      \"description\": \"Release notes content\",\n      \"properties\": {\n        \"syntax\": {\n          \"type\": \"string\",\n          \"description\": \"Format of the release notes content\",\n          \"enum\": [\n            \"plain_text\",\n            \"markdown\",\n            \"asciidoc\"\n          ]\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Release notes text\"\n        }\n      }\n    },\n    \"source_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of source used to create the release bundle\",\n      \"enum\": [\n        \"artifacts\",\n        \"builds\",\n        \"release_bundles\"\
  ,\n        \"aql\"\n      ]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\"\n    },\n    \"created_by\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the release bundle\"\n    },\n    \"artifacts\": {\n      \"type\": \"array\",\n      \"description\": \"Artifacts included in the release bundle\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"source_repo_path\": {\n            \"type\": \"string\",\n            \"description\": \"Original repository path\"\n          },\n          \"target_repo_path\": {\n            \"type\": \"string\",\n            \"description\": \"Target repository path for distribution\"\n          },\n          \"sha256\": {\n            \"type\": \"string\",\n            \"description\": \"SHA-256 checksum\"\n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\"\
  : \"Artifact size in bytes\"\n          },\n          \"props\": {\n            \"type\": \"array\",\n            \"description\": \"Properties attached to the artifact\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"key\": {\n                  \"type\": \"string\"\n                },\n                \"values\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"current_environment\": {\n      \"type\": \"string\",\n      \"description\": \"Current promotion environment\",\n      \"examples\": [\n        \"DEV\",\n        \"STAGING\",\n        \"PROD\"\n      ]\n    },\n    \"promotion_history\": {\n      \"type\": \"array\",\n      \"description\": \"History of environment promotions\",\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"properties\": {\n          \"environment\": {\n            \"type\": \"string\"\n          },\n          \"promoted_at\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"promoted_by\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"COMPLETED\",\n              \"IN_PROGRESS\",\n              \"FAILED\"\n            ]\n          }\n        }\n      }\n    },\n    \"distribution_status\": {\n      \"type\": \"object\",\n      \"description\": \"Distribution status to edge nodes\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Not distributed\",\n            \"In progress\",\n            \"Completed\",\n            \"Failed\"\n          ]\n        },\n        \"sites\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\"\
  : \"object\",\n            \"properties\": {\n              \"site_name\": {\n                \"type\": \"string\"\n              },\n              \"status\": {\n                \"type\": \"string\"\n              },\n              \"distributed_at\": {\n                \"type\": \"string\",\n                \"format\": \"date-time\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"evidence\": {\n      \"type\": \"array\",\n      \"description\": \"Evidence and attestations attached to this release\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"evidence_type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"test_results\",\n              \"approval\",\n              \"scan_results\",\n              \"build_info\",\n              \"custom\"\n            ]\n          },\n          \"description\": {\n         \
  \   \"type\": \"string\"\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"created_by\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"version\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-release-bundle-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Release Bundle
---
