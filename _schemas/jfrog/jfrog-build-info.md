---
description: Represents build information stored in JFrog Artifactory, capturing the complete record of a CI/CD build including source modules, produced artifacts, dependencies, and environment details.
layout: schema
name: JFrog Build Info
properties_list:
- description: Build info schema version
  name: version
  type: string
- description: Build name
  name: name
  type: string
- description: Build number or run identifier
  name: number
  type: string
- description: Type of build system
  name: type
  type: string
- description: Build start timestamp
  name: started
  type: string
- description: Build duration in milliseconds
  name: durationMillis
  type: integer
- description: Build agent information
  name: buildAgent
  type: object
- description: CI server agent information
  name: agent
  type: object
- description: User that triggered the build
  name: principal
  type: string
- description: Artifactory user for publishing build info
  name: artifactoryPrincipal
  type: string
- description: VCS revision (commit hash)
  name: vcsRevision
  type: string
- description: VCS repository URL
  name: vcsUrl
  type: string
- description: CI build URL
  name: url
  type: string
- description: Build modules produced by this build
  name: modules
  type: array
- description: Build promotion statuses
  name: statuses
  type: array
- description: Custom build properties
  name: properties
  type: object
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-build-info-schema.json
slug: jfrog-build-info
source_filename: jfrog-build-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/build-info\",\n  \"title\": \"JFrog Build Info\",\n  \"description\": \"Represents build information stored in JFrog Artifactory, capturing the complete record of a CI/CD build including source modules, produced artifacts, dependencies, and environment details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Build info schema version\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Build name\",\n      \"examples\": [\n        \"my-app-build\"\n      ]\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Build number or run identifier\",\n      \"examples\": [\n        \"42\",\n        \"2025.01.15.1\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of build system\",\n      \"enum\": [\n\
  \        \"GENERIC\",\n        \"MAVEN\",\n        \"GRADLE\",\n        \"ANT\",\n        \"IVY\",\n        \"DOCKER\",\n        \"NPM\",\n        \"NUGET\",\n        \"GO\",\n        \"PIP\"\n      ]\n    },\n    \"started\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Build start timestamp\"\n    },\n    \"durationMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"Build duration in milliseconds\",\n      \"minimum\": 0\n    },\n    \"buildAgent\": {\n      \"type\": \"object\",\n      \"description\": \"Build agent information\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"examples\": [\n            \"Jenkins\",\n            \"GitHub Actions\",\n            \"JFrog Pipelines\"\n          ]\n        },\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"agent\": {\n      \"type\": \"object\",\n      \"description\": \"CI server agent information\"\
  ,\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"version\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"principal\": {\n      \"type\": \"string\",\n      \"description\": \"User that triggered the build\"\n    },\n    \"artifactoryPrincipal\": {\n      \"type\": \"string\",\n      \"description\": \"Artifactory user for publishing build info\"\n    },\n    \"vcsRevision\": {\n      \"type\": \"string\",\n      \"description\": \"VCS revision (commit hash)\"\n    },\n    \"vcsUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"VCS repository URL\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"CI build URL\"\n    },\n    \"modules\": {\n      \"type\": \"array\",\n      \"description\": \"Build modules produced by this build\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Module\"\n      }\n    },\n    \"\
  statuses\": {\n      \"type\": \"array\",\n      \"description\": \"Build promotion statuses\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PromotionStatus\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Custom build properties\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"number\",\n    \"started\"\n  ],\n  \"$defs\": {\n    \"Module\": {\n      \"type\": \"object\",\n      \"description\": \"A build module representing a produced component\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Module identifier\"\n        },\n        \"artifacts\": {\n          \"type\": \"array\",\n          \"description\": \"Artifacts produced by this module\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\"\
  ,\n                \"description\": \"Artifact type/extension\"\n              },\n              \"sha1\": {\n                \"type\": \"string\"\n              },\n              \"sha256\": {\n                \"type\": \"string\"\n              },\n              \"md5\": {\n                \"type\": \"string\"\n              },\n              \"name\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"dependencies\": {\n          \"type\": \"array\",\n          \"description\": \"Dependencies consumed by this module\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\"\n              },\n              \"sha1\": {\n                \"type\": \"string\"\n              },\n              \"sha256\": {\n                \"type\": \"string\"\n              },\n              \"md5\": {\n                \"type\": \"string\"\n        \
  \      },\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"scopes\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"PromotionStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Build promotion status record\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Promotion status name\",\n          \"examples\": [\n            \"staged\",\n            \"released\"\n          ]\n        },\n        \"comment\": {\n          \"type\": \"string\"\n        },\n        \"repository\": {\n          \"type\": \"string\",\n          \"description\": \"Target repository for promotion\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"\
  format\": \"date-time\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"User who performed the promotion\"\n        },\n        \"ciUser\": {\n          \"type\": \"string\",\n          \"description\": \"CI user who triggered the promotion\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-build-info-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Build Info
---
