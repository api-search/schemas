---
description: Details about a beta appliance software update.
layout: schema
name: AlternateSoftwareMetadata
properties_list:
- description: ''
  name: Version
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-alternate-software-metadata-schema.json
slug: openapi-alternate-software-metadata
source_filename: openapi-alternate-software-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-alternate-software-metadata-schema.json\",\n  \"title\": \"AlternateSoftwareMetadata\",\n  \"description\": \"Details about a beta appliance software update.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The appliance software version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-alternate-software-metadata-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: AlternateSoftwareMetadata
---
