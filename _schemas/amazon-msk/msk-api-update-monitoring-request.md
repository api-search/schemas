---
description: Request body for UpdateMonitoring.
layout: schema
name: UpdateMonitoringRequest
properties_list:
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: EnhancedMonitoring
  type: object
- description: ''
  name: OpenMonitoring
  type: object
- description: ''
  name: LoggingInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-monitoring-request-schema.json
slug: msk-api-update-monitoring-request
source_filename: msk-api-update-monitoring-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-monitoring-request-schema.json\",\n  \"title\": \"UpdateMonitoringRequest\",\n  \"description\": \"Request body for UpdateMonitoring.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"currentVersion\"\n          },\n          \"description\": \"\\n            <p>The version of the MSK cluster to update. Cluster versions aren't simple numbers. You can describe an MSK cluster to find its version. When this update operation is successful, it generates a new cluster version.</p>\"\n        }\n      ]\n    },\n    \"EnhancedMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnhancedMonitoring\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"enhancedMonitoring\"\n          },\n          \"description\": \"\\n            <p>Specifies which Apache Kafka metrics Amazon MSK gathers and sends to Amazon CloudWatch for this cluster.</p>\"\n        }\n      ]\n    },\n    \"OpenMonitoring\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenMonitoringInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"openMonitoring\"\n          },\n          \"description\": \"\\n            <p>The settings for open monitoring.</p>\"\n        }\n      ]\n    },\n    \"LoggingInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"loggingInfo\"\n          }\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CurrentVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-monitoring-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: UpdateMonitoringRequest
---
