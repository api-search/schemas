---
description: A collection of fields identifying the service in a response time warning.
layout: schema
name: ResponseTimeRootCauseService
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Names
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: EntityPath
  type: object
- description: ''
  name: Inferred
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-response-time-root-cause-service-schema.json
slug: xray-response-time-root-cause-service
source_filename: xray-response-time-root-cause-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The service name.\"\n        }\n      ]\n    },\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceNames\"\n        },\n        {\n          \"description\": \"A collection of associated service names.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type associated to the service.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The account ID associated to the service.\"\n        }\n      ]\n    },\n    \"EntityPath\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/ResponseTimeRootCauseEntityPath\"\n        },\n        {\n          \"description\": \"The path of root cause entities found on the service. \"\n        }\n      ]\n    },\n    \"Inferred\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableBoolean\"\n        },\n        {\n          \"description\": \"A Boolean value indicating if the service is inferred from the trace.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A collection of fields identifying the service in a response time warning.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseTimeRootCauseService\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-response-time-root-cause-service-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-response-time-root-cause-service-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: ResponseTimeRootCauseService
---
