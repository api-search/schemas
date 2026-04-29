---
description: 'Specifies the Auto-Tune options: the Auto-Tune desired state for the domain, rollback state when disabling Auto-Tune options and list of maintenance schedules.'
layout: schema
name: AutoTuneOptions
properties_list:
- description: ''
  name: DesiredState
  type: object
- description: ''
  name: RollbackOnDisable
  type: object
- description: ''
  name: MaintenanceSchedules
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-options-schema.json
slug: openapi-auto-tune-options
source_filename: openapi-auto-tune-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-options-schema.json\",\n  \"title\": \"AutoTuneOptions\",\n  \"description\": \"Specifies the Auto-Tune options: the Auto-Tune desired state for the domain, rollback state when disabling Auto-Tune options and list of maintenance schedules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DesiredState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneDesiredState\"\n        },\n        {\n          \"description\": \"Specifies the Auto-Tune desired state. Valid values are ENABLED, DISABLED. \"\n        }\n      ]\n    },\n    \"RollbackOnDisable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RollbackOnDisable\"\n        },\n        {\n          \"description\": \"Specifies the rollback state while disabling\
  \ Auto-Tune for the domain. Valid values are NO_ROLLBACK, DEFAULT_ROLLBACK. \"\n        }\n      ]\n    },\n    \"MaintenanceSchedules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneMaintenanceScheduleList\"\n        },\n        {\n          \"description\": \"Specifies list of maitenance schedules. See the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a> for more information.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AutoTuneOptions
---
