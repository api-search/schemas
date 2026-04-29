---
description: Information about an HTTP request.
layout: schema
name: Http
properties_list:
- description: ''
  name: HttpURL
  type: object
- description: ''
  name: HttpStatus
  type: object
- description: ''
  name: HttpMethod
  type: object
- description: ''
  name: UserAgent
  type: object
- description: ''
  name: ClientIp
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-http-schema.json
slug: xray-http
source_filename: xray-http-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpURL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The request URL.\"\n        }\n      ]\n    },\n    \"HttpStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The response status.\"\n        }\n      ]\n    },\n    \"HttpMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The request method.\"\n        }\n      ]\n    },\n    \"UserAgent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The request's user agent string.\"\n        }\n      ]\n    },\n    \"ClientIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"The IP address of the requestor.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about an HTTP request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Http\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-http-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-http-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Http
---
