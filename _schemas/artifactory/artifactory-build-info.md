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
source_filename: artifactory-build-info.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/artifactory-build-info.json\",\n  \"title\": \"Artifactory Build Info\",\n  \"description\": \"Schema for JFrog Artifactory build information, representing a CI/CD build record including modules, artifacts, dependencies, and environment details.\",\n  \"type\": \"object\",\n  \"required\": [\"version\", \"name\", \"number\", \"started\"],\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Build info JSON schema version.\",\n      \"examples\": [\"1.0.1\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Build name identifier.\",\n      \"examples\": [\"my-application\"]\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Build number (version string).\",\n      \"examples\": [\"123\", \"1.0.0-SNAPSHOT\"]\n    },\n    \"type\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Build type corresponding to the build tool used.\",\n      \"enum\": [\n        \"GENERIC\",\n        \"MAVEN\",\n        \"GRADLE\",\n        \"IVY\",\n        \"ANT\",\n        \"NPM\",\n        \"NUGET\",\n        \"GO\",\n        \"PIP\",\n        \"DOCKER\"\n      ]\n    },\n    \"agent\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the CI server agent.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Agent name (e.g., Jenkins, TeamCity, GitHub Actions).\",\n          \"examples\": [\"Jenkins\", \"GitHub Actions\"]\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Agent version.\"\n        }\n      }\n    },\n    \"buildAgent\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the build tool agent.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Build tool name (e.g., MAVEN, GRADLE, NPM).\",\n          \"examples\": [\"MAVEN\", \"GRADLE\"]\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Build tool version.\"\n        }\n      }\n    },\n    \"started\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of when the build started.\"\n    },\n    \"durationMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"Build duration in milliseconds.\",\n      \"minimum\": 0\n    },\n    \"principal\": {\n      \"type\": \"string\",\n      \"description\": \"The user principal who triggered the build.\"\n    },\n    \"artifactoryPrincipal\": {\n      \"type\": \"string\",\n      \"description\": \"The Artifactory user associated with the build.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the build in the CI server.\"\n    },\n  \
  \  \"vcsRevision\": {\n      \"type\": \"string\",\n      \"description\": \"VCS revision (e.g., Git commit SHA).\",\n      \"examples\": [\"a1b2c3d4e5f6\"]\n    },\n    \"vcsUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"VCS repository URL.\"\n    },\n    \"vcs\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed VCS information for multi-module builds.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"revision\": {\n            \"type\": \"string\",\n            \"description\": \"VCS revision/commit.\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"VCS repository URL.\"\n          },\n          \"branch\": {\n            \"type\": \"string\",\n            \"description\": \"VCS branch name.\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Commit message.\"\n          }\n        }\n      }\n    },\n    \"modules\": {\n      \"type\": \"array\",\n      \"description\": \"Build modules, each representing a logical unit of the build.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/module\"\n      }\n    },\n    \"statuses\": {\n      \"type\": \"array\",\n      \"description\": \"Build promotion status history.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/status\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Build-level custom properties.\"\n    },\n    \"buildDependencies\": {\n      \"type\": \"array\",\n      \"description\": \"Other builds this build depends on.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the dependency build.\"\n          },\n     \
  \     \"number\": {\n            \"type\": \"string\",\n            \"description\": \"Number of the dependency build.\"\n          },\n          \"started\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Start time of the dependency build.\"\n          }\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"module\": {\n      \"type\": \"object\",\n      \"description\": \"A build module representing a logical unit (e.g., a Maven module).\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Module identifier (e.g., groupId:artifactId:version for Maven).\",\n          \"examples\": [\"com.example:my-module:1.0.0\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Module type.\"\n        },\n        \"artifacts\": {\n          \"type\": \"array\",\n          \"description\": \"Artifacts produced by this module.\",\n    \
  \      \"items\": {\n            \"$ref\": \"#/$defs/artifact\"\n          }\n        },\n        \"dependencies\": {\n          \"type\": \"array\",\n          \"description\": \"Dependencies consumed by this module.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/dependency\"\n          }\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Module-level custom properties.\"\n        }\n      }\n    },\n    \"artifact\": {\n      \"type\": \"object\",\n      \"description\": \"An artifact produced by a build module.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Artifact type/extension.\",\n          \"examples\": [\"jar\", \"pom\", \"war\", \"tar.gz\"]\n        },\n        \"sha1\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-1 checksum.\",\n       \
  \   \"pattern\": \"^[a-f0-9]{40}$\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 checksum.\",\n          \"pattern\": \"^[a-f0-9]{64}$\"\n        },\n        \"md5\": {\n          \"type\": \"string\",\n          \"description\": \"MD5 checksum.\",\n          \"pattern\": \"^[a-f0-9]{32}$\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Artifact file name.\",\n          \"examples\": [\"my-module-1.0.0.jar\"]\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Artifact-level properties.\"\n        }\n      }\n    },\n    \"dependency\": {\n      \"type\": \"object\",\n      \"description\": \"A dependency consumed by a build module.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"\
  Dependency type/extension.\",\n          \"examples\": [\"jar\", \"pom\"]\n        },\n        \"sha1\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-1 checksum.\",\n          \"pattern\": \"^[a-f0-9]{40}$\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 checksum.\",\n          \"pattern\": \"^[a-f0-9]{64}$\"\n        },\n        \"md5\": {\n          \"type\": \"string\",\n          \"description\": \"MD5 checksum.\",\n          \"pattern\": \"^[a-f0-9]{32}$\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Dependency identifier.\",\n          \"examples\": [\"org.apache.commons:commons-lang3:3.12.0\"]\n        },\n        \"scopes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Dependency scopes.\",\n          \"examples\": [[\"compile\", \"runtime\"]]\n        },\n \
  \       \"requestedBy\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"description\": \"Dependency path showing which modules requested this dependency.\"\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"description\": \"A build promotion status record.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Promotion status label.\",\n          \"examples\": [\"Staged\", \"Released\", \"Rolled-back\"]\n        },\n        \"comment\": {\n          \"type\": \"string\",\n          \"description\": \"Comment associated with the status change.\"\n        },\n        \"repository\": {\n          \"type\": \"string\",\n          \"description\": \"Target repository for this promotion.\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"date-time\",\n          \"description\": \"When the status was applied.\"\n        },\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"Artifactory user who applied the status.\"\n        },\n        \"ciUser\": {\n          \"type\": \"string\",\n          \"description\": \"CI server user who triggered the promotion.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/json-schema/artifactory-build-info.json
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
