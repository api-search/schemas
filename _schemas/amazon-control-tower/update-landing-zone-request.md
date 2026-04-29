---
description: UpdateLandingZoneRequest schema from AWS Control Tower API
layout: schema
name: UpdateLandingZoneRequest
properties_list:
- description: The identifier of the landing zone.
  name: landingZoneIdentifier
  type: string
- description: The landing zone manifest document.
  name: manifest
  type: object
- description: The target landing zone version.
  name: version
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/update-landing-zone-request-schema.json
slug: update-landing-zone-request
source_filename: update-landing-zone-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/update-landing-zone-request-schema.json\",\n  \"title\": \"UpdateLandingZoneRequest\",\n  \"description\": \"UpdateLandingZoneRequest schema from AWS Control Tower API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"landingZoneIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the landing zone.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:landingzone/a1b2c3d4EXAMPLE\"\n    },\n    \"manifest\": {\n      \"type\": \"object\",\n      \"description\": \"The landing zone manifest document.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The target landing zone version.\",\n      \"example\": \"3.3\"\n    }\n  },\n  \"required\": [\n    \"landingZoneIdentifier\",\n    \"manifest\",\n    \"version\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/update-landing-zone-request-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: UpdateLandingZoneRequest
---
