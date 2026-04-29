---
description: A collection of segments and corresponding subsegments associated to a response time warning.
layout: schema
name: ResponseTimeRootCauseEntity
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Coverage
  type: object
- description: ''
  name: Remote
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-response-time-root-cause-entity-schema.json
slug: xray-response-time-root-cause-entity
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the entity.\"\n        }\n      ]\n    },\n    \"Coverage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"The type and messages of the exceptions.\"\n        }\n      ]\n    },\n    \"Remote\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"A flag that denotes a remote subsegment.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A collection of segments and corresponding subsegments associated to a response time warning.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseTimeRootCauseEntity\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-response-time-root-cause-entity-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-response-time-root-cause-entity-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ResponseTimeRootCauseEntity
---
