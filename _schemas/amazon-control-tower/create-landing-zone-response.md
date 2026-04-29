---
description: CreateLandingZoneResponse schema from AWS Control Tower API
layout: schema
name: CreateLandingZoneResponse
properties_list:
- description: The ARN of the landing zone resource.
  name: arn
  type: string
- description: A unique identifier assigned to a CreateLandingZone operation.
  name: operationIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/create-landing-zone-response-schema.json
slug: create-landing-zone-response
source_filename: create-landing-zone-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/create-landing-zone-response-schema.json\",\n  \"title\": \"CreateLandingZoneResponse\",\n  \"description\": \"CreateLandingZoneResponse schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the landing zone resource.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:landingzone/a1b2c3d4EXAMPLE\"\n    },\n    \"operationIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier assigned to a CreateLandingZone operation.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-EXAMPLE11111\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/create-landing-zone-response-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: CreateLandingZoneResponse
---
