---
description: BatchDisassociateProjectAssetsResponse schema
layout: schema
name: BatchDisassociateProjectAssetsResponse
properties_list:
- description: ''
  name: errors
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-batch-disassociate-project-assets-response-schema.json
slug: iot-sitewise-batch-disassociate-project-assets-response
source_filename: iot-sitewise-batch-disassociate-project-assets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-disassociate-project-assets-response-schema.json\",\n  \"title\": \"BatchDisassociateProjectAssetsResponse\",\n  \"description\": \"BatchDisassociateProjectAssetsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchDisassociateProjectAssetsErrors\"\n        },\n        {\n          \"description\": \"A list of associated error information, if any.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-batch-disassociate-project-assets-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: BatchDisassociateProjectAssetsResponse
---
