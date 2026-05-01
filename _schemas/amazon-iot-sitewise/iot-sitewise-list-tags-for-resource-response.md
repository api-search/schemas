---
description: ListTagsForResourceResponse schema
layout: schema
name: ListTagsForResourceResponse
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-list-tags-for-resource-response-schema.json
slug: iot-sitewise-list-tags-for-resource-response
source_filename: iot-sitewise-list-tags-for-resource-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-tags-for-resource-response-schema.json\",\n  \"title\": \"ListTagsForResourceResponse\",\n  \"description\": \"ListTagsForResourceResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of key-value pairs that contain metadata for the resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/tag-resources.html\\\">Tagging your IoT SiteWise resources</a> in the <i>IoT SiteWise User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-list-tags-for-resource-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: ListTagsForResourceResponse
---
