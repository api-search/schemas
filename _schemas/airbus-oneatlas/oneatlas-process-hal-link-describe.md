---
description: ''
layout: schema
name: processHALLinkDescribe
properties_list: []
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-process-hal-link-describe-schema.json
slug: oneatlas-process-hal-link-describe
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-link-describe-schema.json\",\n  \"title\": \"processHALLinkDescribe\",\n  \"allOf\": [\n    {\n      \"properties\": {\n        \"execution\": {\n          \"allOf\": [\n            {\n              \"description\": \"See [Create processing job](#/paths/~1api~1v1~1processes~1{processId}~1jobs/post)\"\n            },\n            {\n              \"$ref\": \"#/components/schemas/Link\"\n            }\n          ]\n        },\n        \"self\": {\n          \"$ref\": \"#/components/schemas/Link\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/processHALLinkCommon\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-link-describe-schema.json
tags:
- Imagery
- Satellites
title: processHALLinkDescribe
---
