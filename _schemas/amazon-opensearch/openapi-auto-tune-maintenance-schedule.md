---
description: Specifies Auto-Tune maitenance schedule. See the <a href="https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html" target="_blank">Developer Guide</a> for more information.
layout: schema
name: AutoTuneMaintenanceSchedule
properties_list:
- description: ''
  name: StartAt
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: CronExpressionForRecurrence
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-maintenance-schedule-schema.json
slug: openapi-auto-tune-maintenance-schedule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-maintenance-schedule-schema.json\",\n  \"title\": \"AutoTuneMaintenanceSchedule\",\n  \"description\": \"Specifies Auto-Tune maitenance schedule. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StartAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartAt\"\n        },\n        {\n          \"description\": \"Specifies timestamp at which Auto-Tune maintenance schedule start. \"\n        }\n      ]\n    },\n    \"Duration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Duration\"\n        },\n        {\n          \"description\": \"Specifies\
  \ maintenance schedule duration: duration value and duration unit. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information.\"\n        }\n      ]\n    },\n    \"CronExpressionForRecurrence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Specifies cron expression for a recurring maintenance schedule. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-maintenance-schedule-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AutoTuneMaintenanceSchedule
---
