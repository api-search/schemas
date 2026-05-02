---
description: Represents an artifact stored in a JFrog Artifactory repository, including its metadata, checksums, and storage properties.
layout: schema
name: JFrog Artifact
properties_list:
- description: Repository key where the artifact is stored
  name: repo
  type: string
- description: Path to the artifact within the repository
  name: path
  type: string
- description: Name of the artifact file
  name: name
  type: string
- description: Type of item (file or folder)
  name: type
  type: string
- description: Timestamp when the artifact was created
  name: created
  type: string
- description: Username that created the artifact
  name: createdBy
  type: string
- description: Timestamp of last modification
  name: lastModified
  type: string
- description: Username that last modified the artifact
  name: modifiedBy
  type: string
- description: Timestamp of last metadata update
  name: lastUpdated
  type: string
- description: Direct download URI for the artifact
  name: downloadUri
  type: string
- description: MIME type of the artifact
  name: mimeType
  type: string
- description: Size of the artifact in bytes
  name: size
  type: integer
- description: ''
  name: checksums
  type: object
- description: ''
  name: originalChecksums
  type: object
- description: Custom properties attached to the artifact
  name: properties
  type: object
- description: REST API URI for this artifact info
  name: uri
  type: string
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-artifact-schema.json
slug: jfrog-artifact
source_filename: jfrog-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/artifact\",\n  \"title\": \"JFrog Artifact\",\n  \"description\": \"Represents an artifact stored in a JFrog Artifactory repository, including its metadata, checksums, and storage properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repo\": {\n      \"type\": \"string\",\n      \"description\": \"Repository key where the artifact is stored\",\n      \"examples\": [\n        \"libs-release-local\",\n        \"npm-remote\"\n      ]\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the artifact within the repository\",\n      \"examples\": [\n        \"org/example/my-artifact/1.0.0/my-artifact-1.0.0.jar\"\n      ]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the artifact file\",\n      \"examples\": [\n        \"my-artifact-1.0.0.jar\"\n      ]\n    },\n    \"type\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Type of item (file or folder)\",\n      \"enum\": [\n        \"file\",\n        \"folder\"\n      ]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the artifact was created\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username that created the artifact\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last modification\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username that last modified the artifact\"\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last metadata update\"\n    },\n    \"downloadUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Direct download\
  \ URI for the artifact\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the artifact\",\n      \"examples\": [\n        \"application/java-archive\",\n        \"application/gzip\",\n        \"application/json\"\n      ]\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the artifact in bytes\"\n    },\n    \"checksums\": {\n      \"$ref\": \"#/$defs/Checksums\"\n    },\n    \"originalChecksums\": {\n      \"$ref\": \"#/$defs/Checksums\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Custom properties attached to the artifact\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"REST API URI for this artifact info\"\n    }\n  },\n  \"required\": [\n    \"repo\",\n    \"\
  path\",\n    \"name\"\n  ],\n  \"$defs\": {\n    \"Checksums\": {\n      \"type\": \"object\",\n      \"description\": \"Cryptographic checksums for the artifact\",\n      \"properties\": {\n        \"sha1\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-f0-9]{40}$\",\n          \"description\": \"SHA-1 checksum\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-f0-9]{64}$\",\n          \"description\": \"SHA-256 checksum\"\n        },\n        \"md5\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-f0-9]{32}$\",\n          \"description\": \"MD5 checksum\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-artifact-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Artifact
---
