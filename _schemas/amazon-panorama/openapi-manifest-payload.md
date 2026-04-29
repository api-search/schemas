---
description: A application verion's manifest file. This is a JSON document that has a single key (<code>PayloadData</code>) where the value is an escaped string representation of the application manifest (<code>graph.json</code>). This file is located in the <code>graphs</code> folder in your application source.
layout: schema
name: ManifestPayload
properties_list:
- description: ''
  name: PayloadData
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-manifest-payload-schema.json
slug: openapi-manifest-payload
source_filename: openapi-manifest-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-manifest-payload-schema.json\",\n  \"title\": \"ManifestPayload\",\n  \"description\": \"A application verion's manifest file. This is a JSON document that has a single key (<code>PayloadData</code>) where the value is an escaped string representation of the application manifest (<code>graph.json</code>). This file is located in the <code>graphs</code> folder in your application source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PayloadData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestPayloadData\"\n        },\n        {\n          \"description\": \"The application manifest.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-manifest-payload-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ManifestPayload
---
