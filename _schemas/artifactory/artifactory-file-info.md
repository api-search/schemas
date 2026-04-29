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
source_filename: artifactory-file-info.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/artifactory-file-info.json\",\n  \"title\": \"Artifactory File Info\",\n  \"description\": \"Schema for artifact file information returned by the Artifactory storage API, including metadata, checksums, and download URI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repo\": {\n      \"type\": \"string\",\n      \"description\": \"Repository key where the file is stored.\",\n      \"examples\": [\"libs-release-local\"]\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the file within the repository.\",\n      \"examples\": [\"/org/example/mylib/1.0/mylib-1.0.jar\"]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the file was first created.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username\
  \ of the user who created/deployed the file.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last modification.\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who last modified the file.\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last update (including metadata changes).\"\n    },\n    \"downloadUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Direct download URI for the artifact.\"\n    },\n    \"remoteUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Remote URL if this is a cached remote artifact.\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the file.\",\n      \"examples\": [\"application/java-archive\"\
  , \"application/octet-stream\", \"text/xml\"]\n    },\n    \"size\": {\n      \"type\": [\"string\", \"integer\"],\n      \"description\": \"File size in bytes. May be returned as a string or integer.\"\n    },\n    \"checksums\": {\n      \"$ref\": \"#/$defs/checksums\",\n      \"description\": \"Checksums computed by Artifactory.\"\n    },\n    \"originalChecksums\": {\n      \"$ref\": \"#/$defs/checksums\",\n      \"description\": \"Checksums as provided during deployment (before Artifactory verification).\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URI for this file info resource.\"\n    }\n  },\n  \"$defs\": {\n    \"checksums\": {\n      \"type\": \"object\",\n      \"description\": \"File checksums in multiple hash algorithms.\",\n      \"properties\": {\n        \"sha1\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-1 hash of the file content.\",\n          \"pattern\": \"^[a-f0-9]{40}$\"\
  \n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 hash of the file content.\",\n          \"pattern\": \"^[a-f0-9]{64}$\"\n        },\n        \"md5\": {\n          \"type\": \"string\",\n          \"description\": \"MD5 hash of the file content.\",\n          \"pattern\": \"^[a-f0-9]{32}$\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/artifactory/refs/heads/main/json-schema/artifactory-file-info.json
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
