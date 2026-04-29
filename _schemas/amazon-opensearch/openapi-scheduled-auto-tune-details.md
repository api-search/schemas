---
description: Specifies details of the scheduled Auto-Tune action. See the <a href="https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html" target="_blank">Developer Guide</a> for more information.
layout: schema
name: ScheduledAutoTuneDetails
properties_list:
- description: ''
  name: Date
  type: object
- description: ''
  name: ActionType
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: Severity
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-scheduled-auto-tune-details-schema.json
slug: openapi-scheduled-auto-tune-details
source_filename: openapi-scheduled-auto-tune-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-scheduled-auto-tune-details-schema.json\",\n  \"title\": \"ScheduledAutoTuneDetails\",\n  \"description\": \"Specifies details of the scheduled Auto-Tune action. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Date\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneDate\"\n        },\n        {\n          \"description\": \"Specifies timestamp for the Auto-Tune action scheduled for the domain. \"\n        }\n      ]\n    },\n    \"ActionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAutoTuneActionType\"\n        },\n        {\n \
  \         \"description\": \"Specifies Auto-Tune action type. Valid values are JVM_HEAP_SIZE_TUNING and JVM_YOUNG_GEN_TUNING. \"\n        }\n      ]\n    },\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAutoTuneDescription\"\n        },\n        {\n          \"description\": \"Specifies Auto-Tune action description. \"\n        }\n      ]\n    },\n    \"Severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAutoTuneSeverityType\"\n        },\n        {\n          \"description\": \"Specifies Auto-Tune action severity. Valid values are LOW, MEDIUM and HIGH. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-scheduled-auto-tune-details-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ScheduledAutoTuneDetails
---
