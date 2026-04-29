---
description: <p/>
layout: schema
name: BackendConnectionErrors
properties_list:
- description: ''
  name: TimeoutCount
  type: object
- description: ''
  name: ConnectionRefusedCount
  type: object
- description: ''
  name: HTTPCode4XXCount
  type: object
- description: ''
  name: HTTPCode5XXCount
  type: object
- description: ''
  name: UnknownHostCount
  type: object
- description: ''
  name: OtherCount
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-backend-connection-errors-schema.json
slug: xray-backend-connection-errors
source_filename: xray-backend-connection-errors-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeoutCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"ConnectionRefusedCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"HTTPCode4XXCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"HTTPCode5XXCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"UnknownHostCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\
  \n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"OtherCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p/>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BackendConnectionErrors\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-backend-connection-errors-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-backend-connection-errors-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: BackendConnectionErrors
---
