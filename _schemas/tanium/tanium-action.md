---
description: Represents an action deployed to endpoints through the Tanium platform. Actions execute packages on targeted endpoint groups for remediation, software deployment, configuration changes, or compliance enforcement.
layout: schema
name: Tanium Action
properties_list:
- description: Unique numeric identifier for the action
  name: id
  type: integer
- description: Name of the action
  name: name
  type: string
- description: Current execution status of the action
  name: status
  type: string
- description: Package specification deployed by this action
  name: packageSpec
  type: object
- description: Action group governing approval and targeting
  name: actionGroup
  type: object
- description: Computer group targeted by this action
  name: targetGroup
  type: object
- description: Scheduled or actual start time of the action
  name: startTime
  type: string
- description: Expiration time after which the action stops deploying
  name: expirationTime
  type: string
- description: Whether the action has been approved (1 for approved)
  name: approvedFlag
  type: integer
- description: Seconds until the action expires
  name: expireSeconds
  type: integer
provider_name: Tanium
provider_slug: tanium
schema_file: json-schema/tanium-action-schema.json
slug: tanium-action
source_filename: tanium-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/tanium/blob/main/json-schema/tanium-action-schema.json\",\n  \"title\": \"Tanium Action\",\n  \"description\": \"Represents an action deployed to endpoints through the Tanium platform. Actions execute packages on targeted endpoint groups for remediation, software deployment, configuration changes, or compliance enforcement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the action\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the action\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current execution status of the action\"\n    },\n    \"packageSpec\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"sourceId\": {\n          \"type\": \"integer\",\n          \"\
  description\": \"Package identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Package name\"\n        },\n        \"parameters\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"key\": {\n                \"type\": \"string\",\n                \"description\": \"Parameter key\"\n              },\n              \"value\": {\n                \"type\": \"string\",\n                \"description\": \"Parameter value\"\n              }\n            }\n          },\n          \"description\": \"Package parameters for this action\"\n        }\n      },\n      \"description\": \"Package specification deployed by this action\"\n    },\n    \"actionGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Action group identifier\"\n        },\n        \"name\":\
  \ {\n          \"type\": \"string\",\n          \"description\": \"Action group name\"\n        }\n      },\n      \"description\": \"Action group governing approval and targeting\"\n    },\n    \"targetGroup\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Target group identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Target group name\"\n        }\n      },\n      \"description\": \"Computer group targeted by this action\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Scheduled or actual start time of the action\"\n    },\n    \"expirationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Expiration time after which the action stops deploying\"\n    },\n    \"approvedFlag\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Whether the action has been approved (1 for approved)\"\n    },\n    \"expireSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Seconds until the action expires\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/json-schema/tanium-action-schema.json
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
title: Tanium Action
---
