---
description: CreateLandingZoneRequest schema from AWS Control Tower API
layout: schema
name: CreateLandingZoneRequest
properties_list:
- description: The landing zone manifest document, a YAML expressible input type.
  name: manifest
  type: object
- description: The landing zone version, for example, 3.3.
  name: version
  type: string
- description: Tags to apply to the landing zone.
  name: tags
  type: object
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/create-landing-zone-request-schema.json
slug: create-landing-zone-request
source_filename: create-landing-zone-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/create-landing-zone-request-schema.json\",\n  \"title\": \"CreateLandingZoneRequest\",\n  \"description\": \"CreateLandingZoneRequest schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"manifest\": {\n      \"type\": \"object\",\n      \"description\": \"The landing zone manifest document, a YAML expressible input type.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The landing zone version, for example, 3.3.\",\n      \"example\": \"3.3\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags to apply to the landing zone.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"manifest\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/create-landing-zone-request-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: CreateLandingZoneRequest
---
