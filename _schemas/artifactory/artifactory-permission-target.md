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
source_filename: artifactory-permission-target.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/artifactory-permission-target.json\",\n  \"title\": \"Artifactory Permission Target\",\n  \"description\": \"Schema for JFrog Artifactory permission targets (V2), defining access control rules for repositories and builds. Permission targets map users and groups to specific permissions on repository and build resources.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the permission target.\",\n      \"examples\": [\"release-deployers\", \"dev-team-access\"]\n    },\n    \"repo\": {\n      \"$ref\": \"#/$defs/permissionSection\",\n      \"description\": \"Repository permissions section defining access to repository artifacts.\"\n    },\n    \"build\": {\n      \"$ref\": \"#/$defs/permissionSection\",\n      \"description\": \"Build permissions section defining\
  \ access to build information.\"\n    }\n  },\n  \"$defs\": {\n    \"permissionSection\": {\n      \"type\": \"object\",\n      \"description\": \"A permission section for either repositories or builds.\",\n      \"properties\": {\n        \"repositories\": {\n          \"type\": \"array\",\n          \"description\": \"List of repository or build repository keys this permission applies to. Use 'ANY' for all repositories, 'ANY LOCAL' for all local repos, 'ANY REMOTE' for all remote repos.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"examples\": [\n            [\"libs-release-local\", \"libs-snapshot-local\"],\n            [\"ANY\"],\n            [\"ANY LOCAL\"]\n          ]\n        },\n        \"actions\": {\n          \"type\": \"object\",\n          \"description\": \"Permission actions mapped to users and groups.\",\n          \"properties\": {\n            \"users\": {\n              \"type\": \"object\",\n              \"description\": \"\
  Map of usernames to their permission actions.\",\n              \"additionalProperties\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"$ref\": \"#/$defs/permissionAction\"\n                }\n              },\n              \"examples\": [\n                {\n                  \"admin-user\": [\"manage\", \"read\", \"write\", \"annotate\", \"delete\"],\n                  \"deployer\": [\"read\", \"write\", \"annotate\"]\n                }\n              ]\n            },\n            \"groups\": {\n              \"type\": \"object\",\n              \"description\": \"Map of group names to their permission actions.\",\n              \"additionalProperties\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"$ref\": \"#/$defs/permissionAction\"\n                }\n              },\n              \"examples\": [\n                {\n                  \"dev-team\": [\"read\", \"write\", \"annotate\"],\n \
  \                 \"readers\": [\"read\"]\n                }\n              ]\n            }\n          }\n        },\n        \"includePatterns\": {\n          \"type\": \"array\",\n          \"description\": \"Artifact path patterns to include in this permission scope.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"default\": [\"**\"],\n          \"examples\": [[\"**\"], [\"com/example/**\"]]\n        },\n        \"excludePatterns\": {\n          \"type\": \"array\",\n          \"description\": \"Artifact path patterns to exclude from this permission scope.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"default\": [],\n          \"examples\": [[], [\"com/internal/**\"]]\n        }\n      }\n    },\n    \"permissionAction\": {\n      \"type\": \"string\",\n      \"description\": \"A permission action that can be granted to users or groups.\",\n      \"enum\": [\n        \"read\",\n        \"write\",\n  \
  \      \"annotate\",\n        \"delete\",\n        \"manage\",\n        \"managedXrayMeta\",\n        \"distribute\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/json-schema/artifactory-permission-target.json
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
