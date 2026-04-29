---
description: ''
layout: schema
name: DescribeProcessLinks
properties_list: []
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-describe-process-links-schema.json
slug: oneatlas-describe-process-links
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-describe-process-links-schema.json\",\n  \"title\": \"DescribeProcessLinks\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/processHALLinkCommon\"\n    },\n    {\n      \"properties\": {\n        \"self\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            },\n            {\n              \"description\": \"The resource that return this process description\"\n            }\n          ]\n        }\n      },\n      \"type\": \"object\"\n    },\n    {\n      \"properties\": {\n        \"execution\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Describe process](#/paths/~1api~1v1~1processes~1{processId}/post)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\
  \n            }\n          ]\n        }\n      },\n      \"type\": \"object\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-describe-process-links-schema.json
tags:
- Imagery
- Satellites
title: DescribeProcessLinks
---
