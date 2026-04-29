---
description: An AWS Control Tower landing zone.
layout: schema
name: LandingZone
properties_list:
- description: The ARN of the landing zone.
  name: arn
  type: string
- description: The drift status of the landing zone.
  name: driftStatus
  type: object
- description: The latest available version of the landing zone.
  name: latestAvailableVersion
  type: string
- description: The landing zone manifest document.
  name: manifest
  type: object
- description: The landing zone deployment status.
  name: status
  type: string
- description: The current deployed version of the landing zone.
  name: version
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/landing-zone-schema.json
slug: landing-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-schema.json\",\n  \"title\": \"LandingZone\",\n  \"description\": \"An AWS Control Tower landing zone.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the landing zone.\",\n      \"example\": \"arn:aws:controltower:us-east-1:123456789012:landingzone/a1b2c3d4EXAMPLE\"\n    },\n    \"driftStatus\": {\n      \"type\": \"object\",\n      \"description\": \"The drift status of the landing zone.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"DRIFTED\",\n            \"IN_SYNC\",\n            \"NOT_CHECKING_FOR_DRIFT\",\n            \"UNKNOWN\"\n          ]\n        }\n      }\n    },\n    \"latestAvailableVersion\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The latest available version of the landing zone.\",\n      \"example\": \"3.3\"\n    },\n    \"manifest\": {\n      \"type\": \"object\",\n      \"description\": \"The landing zone manifest document.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The landing zone deployment status.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PROCESSING\",\n        \"FAILED\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The current deployed version of the landing zone.\",\n      \"example\": \"3.3\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: LandingZone
---
