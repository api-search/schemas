---
description: Provides status of the delivery of the snapshot or the configuration history to the specified Amazon S3 bucket. Also provides the status of notifications about the Amazon S3 delivery to the specified Amazon SNS topic.
layout: schema
name: ConfigExportDeliveryInfo
properties_list:
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
  name: lastAttemptTime
  type: object
- description: ''
  name: lastSuccessfulTime
  type: object
- description: ''
  name: nextDeliveryTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-config-export-delivery-info-schema.json
slug: config-config-export-delivery-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-export-delivery-info-schema.json\",\n  \"title\": \"ConfigExportDeliveryInfo\",\n  \"description\": \"Provides status of the delivery of the snapshot or the configuration history to the specified Amazon S3 bucket. Also provides the status of notifications about the Amazon S3 delivery to the specified Amazon SNS topic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryStatus\"\n        },\n        {\n          \"description\": \"Status of the last attempted delivery.\"\n        }\n      ]\n    },\n    \"lastErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error code from the last attempted\
  \ delivery.\"\n        }\n      ]\n    },\n    \"lastErrorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The error message from the last attempted delivery.\"\n        }\n      ]\n    },\n    \"lastAttemptTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time of the last attempted delivery.\"\n        }\n      ]\n    },\n    \"lastSuccessfulTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time of the last successful delivery.\"\n        }\n      ]\n    },\n    \"nextDeliveryTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The time that the next delivery occurs.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-config-export-delivery-info-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigExportDeliveryInfo
---
