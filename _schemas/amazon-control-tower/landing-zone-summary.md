---
description: Summary information about a landing zone.
layout: schema
name: LandingZoneSummary
properties_list:
- description: The ARN of the landing zone.
  name: arn
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/landing-zone-summary-schema.json
slug: landing-zone-summary
source_filename: landing-zone-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-summary-schema.json\",\n  \"title\": \"LandingZoneSummary\",\n  \"description\": \"Summary information about a landing zone.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the landing zone.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:landingzone/a1b2c3d4EXAMPLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-summary-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: LandingZoneSummary
---
