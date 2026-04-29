---
description: Information about the position of the asset in a rack.
layout: schema
name: AssetLocation
properties_list:
- description: ''
  name: RackElevation
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-asset-location-schema.json
slug: openapi-asset-location
source_filename: openapi-asset-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-asset-location-schema.json\",\n  \"title\": \"AssetLocation\",\n  \"description\": \" Information about the position of the asset in a rack. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RackElevation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RackElevation\"\n        },\n        {\n          \"description\": \" The position of an asset in a rack measured in rack units. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-asset-location-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: AssetLocation
---
