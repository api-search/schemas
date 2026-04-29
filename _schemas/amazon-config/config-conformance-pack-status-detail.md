---
description: Status details of a conformance pack.
layout: schema
name: ConformancePackStatusDetail
properties_list:
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: ConformancePackId
  type: object
- description: ''
  name: ConformancePackArn
  type: object
- description: ''
  name: ConformancePackState
  type: object
- description: ''
  name: StackArn
  type: object
- description: ''
  name: ConformancePackStatusReason
  type: object
- description: ''
  name: LastUpdateRequestedTime
  type: object
- description: ''
  name: LastUpdateCompletedTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-status-detail-schema.json
slug: config-conformance-pack-status-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-status-detail-schema.json\",\n  \"title\": \"ConformancePackStatusDetail\",\n  \"description\": \"Status details of a conformance pack.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"Name of the conformance pack.\"\n        }\n      ]\n    },\n    \"ConformancePackId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackId\"\n        },\n        {\n          \"description\": \"ID of the conformance pack.\"\n        }\n      ]\n    },\n    \"ConformancePackArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackArn\"\n\
  \        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of comformance pack.\"\n        }\n      ]\n    },\n    \"ConformancePackState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackState\"\n        },\n        {\n          \"description\": \"<p>Indicates deployment status of conformance pack.</p> <p>Config sets the state of the conformance pack to:</p> <ul> <li> <p>CREATE_IN_PROGRESS when a conformance pack creation is in progress for an account.</p> </li> <li> <p>CREATE_COMPLETE when a conformance pack has been successfully created in your account.</p> </li> <li> <p>CREATE_FAILED when a conformance pack creation failed in your account.</p> </li> <li> <p>DELETE_IN_PROGRESS when a conformance pack deletion is in progress. </p> </li> <li> <p>DELETE_FAILED when a conformance pack deletion failed in your account.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"StackArn\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/StackArn\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of CloudFormation stack. \"\n        }\n      ]\n    },\n    \"ConformancePackStatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackStatusReason\"\n        },\n        {\n          \"description\": \"The reason of conformance pack creation failure.\"\n        }\n      ]\n    },\n    \"LastUpdateRequestedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"Last time when conformation pack creation and update was requested.\"\n        }\n      ]\n    },\n    \"LastUpdateCompletedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"Last time when conformation pack creation and update was successful.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"ConformancePackName\",\n    \"ConformancePackId\",\n    \"ConformancePackArn\",\n    \"ConformancePackState\",\n    \"StackArn\",\n    \"LastUpdateRequestedTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-status-detail-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackStatusDetail
---
