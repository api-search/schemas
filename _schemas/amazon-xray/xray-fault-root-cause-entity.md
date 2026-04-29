---
description: A collection of segments and corresponding subsegments associated to a trace summary fault error.
layout: schema
name: FaultRootCauseEntity
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Exceptions
  type: object
- description: ''
  name: Remote
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-fault-root-cause-entity-schema.json
slug: xray-fault-root-cause-entity
source_filename: xray-fault-root-cause-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the entity.\"\n        }\n      ]\n    },\n    \"Exceptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RootCauseExceptions\"\n        },\n        {\n          \"description\": \"The types and messages of the exceptions.\"\n        }\n      ]\n    },\n    \"Remote\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"A flag that denotes a remote subsegment.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A collection of segments and corresponding subsegments associated to a trace summary fault error.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FaultRootCauseEntity\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-fault-root-cause-entity-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-fault-root-cause-entity-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: FaultRootCauseEntity
---
