---
description: ListLandingZoneOperationsResponse schema from AWS Control Tower API
layout: schema
name: ListLandingZoneOperationsResponse
properties_list:
- description: ''
  name: landingZoneOperations
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/list-landing-zone-operations-response-schema.json
slug: list-landing-zone-operations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-landing-zone-operations-response-schema.json\",\n  \"title\": \"ListLandingZoneOperationsResponse\",\n  \"description\": \"ListLandingZoneOperationsResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"landingZoneOperations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LandingZoneOperationSummary\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/list-landing-zone-operations-response-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: ListLandingZoneOperationsResponse
---
