---
description: the HAL target uri for a process
layout: schema
name: processHALLinkCommon
properties_list:
- description: ''
  name: documentation
  type: object
- description: ''
  name: icon
  type: object
- description: ''
  name: license
  type: object
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-process-hal-link-common-schema.json
slug: oneatlas-process-hal-link-common
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-link-common-schema.json\",\n  \"title\": \"processHALLinkCommon\",\n  \"type\": \"object\",\n  \"description\": \"the HAL target uri for a process\",\n  \"properties\": {\n    \"documentation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Link\"\n        },\n        {\n          \"description\": \"The target resource to retrieve the documentation of this process\"\n        }\n      ]\n    },\n    \"icon\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Link\"\n        },\n        {\n          \"description\": \"The target resource to retrieve the icon of this process\"\n        }\n      ]\n    },\n    \"license\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Link\"\n        },\n        {\n\
  \          \"description\": \"The target resource to retrieve the license of this process\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-process-hal-link-common-schema.json
tags:
- Imagery
- Satellites
title: processHALLinkCommon
---
