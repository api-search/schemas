---
description: Represents a deployment package in the Tanium platform. Packages contain scripts and files that are deployed to endpoints through actions to perform remediation, configuration changes, or software installation.
layout: schema
name: Tanium Package
properties_list:
- description: Unique numeric identifier for the package
  name: id
  type: integer
- description: Package name
  name: name
  type: string
- description: Human-friendly display name
  name: displayName
  type: string
- description: Command line to execute on the endpoint
  name: command
  type: string
- description: Timeout in seconds for command execution
  name: commandTimeout
  type: integer
- description: Seconds until the package action expires
  name: expireSeconds
  type: integer
- description: Content set the package belongs to
  name: contentSet
  type: object
- description: Files included in the package for deployment
  name: files
  type: array
- description: Configurable parameters for the package
  name: parameters
  type: array
- description: Last modification timestamp
  name: modTime
  type: string
- description: Creation timestamp
  name: creationTime
  type: string
provider_name: Tanium
provider_slug: tanium
schema_file: json-schema/tanium-package-schema.json
slug: tanium-package
source_filename: tanium-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/tanium/blob/main/json-schema/tanium-package-schema.json\",\n  \"title\": \"Tanium Package\",\n  \"description\": \"Represents a deployment package in the Tanium platform. Packages contain scripts and files that are deployed to endpoints through actions to perform remediation, configuration changes, or software installation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the package\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Package name\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-friendly display name\"\n    },\n    \"command\": {\n      \"type\": \"string\",\n      \"description\": \"Command line to execute on the endpoint\"\n    },\n    \"commandTimeout\": {\n      \"\
  type\": \"integer\",\n      \"description\": \"Timeout in seconds for command execution\"\n    },\n    \"expireSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds until the package action expires\"\n    },\n    \"contentSet\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Content set identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Content set name\"\n        }\n      },\n      \"description\": \"Content set the package belongs to\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"File identifier\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"File name\"\n          },\n          \"hash\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"File hash for integrity verification\"\n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\": \"File size in bytes\"\n          }\n        }\n      },\n      \"description\": \"Files included in the package for deployment\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"Parameter key name\"\n          },\n          \"defaultValue\": {\n            \"type\": \"string\",\n            \"description\": \"Default parameter value\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable parameter label\"\n          }\n        }\n      },\n      \"description\": \"Configurable parameters for the package\"\n    },\n    \"modTime\": {\n  \
  \    \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/json-schema/tanium-package-schema.json
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
title: Tanium Package
---
