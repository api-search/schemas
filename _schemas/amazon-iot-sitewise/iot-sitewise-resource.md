---
description: Contains an IoT SiteWise Monitor resource ID for a portal or project.
layout: schema
name: Resource
properties_list:
- description: ''
  name: portal
  type: object
- description: ''
  name: project
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-resource-schema.json
slug: iot-sitewise-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"Contains an IoT SiteWise Monitor resource ID for a portal or project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"portal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortalResource\"\n        },\n        {\n          \"description\": \"A portal resource.\"\n        }\n      ]\n    },\n    \"project\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectResource\"\n        },\n        {\n          \"description\": \"A project resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-resource-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: Resource
---
