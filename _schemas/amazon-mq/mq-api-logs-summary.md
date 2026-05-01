---
description: The list of information about logs currently enabled and pending to be deployed for the specified broker.
layout: schema
name: LogsSummary
properties_list:
- description: ''
  name: Audit
  type: object
- description: ''
  name: AuditLogGroup
  type: object
- description: ''
  name: General
  type: object
- description: ''
  name: GeneralLogGroup
  type: object
- description: ''
  name: Pending
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-logs-summary-schema.json
slug: mq-api-logs-summary
source_filename: mq-api-logs-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-logs-summary-schema.json\",\n  \"title\": \"LogsSummary\",\n  \"description\": \"The list of information about logs currently enabled and pending to be deployed for the specified broker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Audit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"audit\"\n          },\n          \"description\": \"Enables audit logging. Every user management action made using JMX or the ActiveMQ Web Console is logged.\"\n        }\n      ]\n    },\n    \"AuditLogGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"auditLogGroup\"\n          },\n\
  \          \"description\": \"The location of the CloudWatch Logs log group where audit logs are sent.\"\n        }\n      ]\n    },\n    \"General\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"general\"\n          },\n          \"description\": \"Enables general logging.\"\n        }\n      ]\n    },\n    \"GeneralLogGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"generalLogGroup\"\n          },\n          \"description\": \"The location of the CloudWatch Logs log group where general logs are sent.\"\n        }\n      ]\n    },\n    \"Pending\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PendingLogs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"pending\"\n          },\n          \"description\"\
  : \"The list of information about logs pending to be deployed for the specified broker.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GeneralLogGroup\",\n    \"General\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-logs-summary-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: LogsSummary
---
