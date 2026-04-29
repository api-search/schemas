---
description: Parameter overrides for an application instance. This is a JSON document that has a single key (<code>PayloadData</code>) where the value is an escaped string representation of the overrides document.
layout: schema
name: ManifestOverridesPayload
properties_list:
- description: ''
  name: PayloadData
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-manifest-overrides-payload-schema.json
slug: openapi-manifest-overrides-payload
source_filename: openapi-manifest-overrides-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-manifest-overrides-payload-schema.json\",\n  \"title\": \"ManifestOverridesPayload\",\n  \"description\": \"Parameter overrides for an application instance. This is a JSON document that has a single key (<code>PayloadData</code>) where the value is an escaped string representation of the overrides document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PayloadData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestOverridesPayloadData\"\n        },\n        {\n          \"description\": \"The overrides document.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-manifest-overrides-payload-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: ManifestOverridesPayload
---
