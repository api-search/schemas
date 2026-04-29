---
description: <p>The current status of the configuration recorder.</p> <note> <p>For a detailed status of recording events over time, add your Config events to CloudWatch metrics and use CloudWatch metrics.</p> </note>
layout: schema
name: ConfigurationRecorderStatus
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: lastStartTime
  type: object
- description: ''
  name: lastStopTime
  type: object
- description: ''
  name: recording
  type: object
- description: ''
  name: lastStatus
  type: object
- description: ''
  name: lastErrorCode
  type: object
- description: ''
  name: lastErrorMessage
  type: object
- description: ''
  name: lastStatusChangeTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-configuration-recorder-status-schema.json
slug: config-configuration-recorder-status
source_filename: config-configuration-recorder-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-recorder-status-schema.json\",\n  \"title\": \"ConfigurationRecorderStatus\",\n  \"description\": \"<p>The current status of the configuration recorder.</p> <note> <p>For a detailed status of recording events over time, add your Config events to CloudWatch metrics and use CloudWatch metrics.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the configuration recorder.\"\n        }\n      ]\n    },\n    \"lastStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time the recorder was last started.\"\n        }\n\
  \      ]\n    },\n    \"lastStopTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time the recorder was last stopped.\"\n        }\n      ]\n    },\n    \"recording\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether or not the recorder is currently recording.\"\n        }\n      ]\n    },\n    \"lastStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecorderStatus\"\n        },\n        {\n          \"description\": \"The status of the latest recording event processed by the recorder.\"\n        }\n      ]\n    },\n    \"lastErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The latest error code from when the recorder last failed.\"\n        }\n\
  \      ]\n    },\n    \"lastErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The latest error message from when the recorder last failed.\"\n        }\n      ]\n    },\n    \"lastStatusChangeTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time of the latest change in status of an recording event processed by the recorder.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-recorder-status-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigurationRecorderStatus
---
