---
description: ListLandingZonesResponse schema from AWS Control Tower API
layout: schema
name: ListLandingZonesResponse
properties_list:
- description: ''
  name: landingZones
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/list-landing-zones-response-schema.json
slug: list-landing-zones-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-landing-zones-response-schema.json\",\n  \"title\": \"ListLandingZonesResponse\",\n  \"description\": \"ListLandingZonesResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"landingZones\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LandingZoneSummary\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-landing-zones-response-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: ListLandingZonesResponse
---
