---
description: A DataSync location representing a source or destination storage system.
layout: schema
name: Location
properties_list:
- description: The ARN of the DataSync location. This ARN uniquely identifies the location.
  name: LocationArn
  type: string
- description: The URL of the location
  name: LocationUri
  type: string
- description: ''
  name: CreationTime
  type: string
provider_name: Amazon DataSync
provider_slug: amazon-datasync
schema_file: json-schema/location-schema.json
slug: location
source_filename: location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-datasync/json-schema/location-schema.json\",\n  \"title\": \"Location\",\n  \"description\": \"A DataSync location representing a source or destination storage system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LocationArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the DataSync location. This ARN uniquely identifies the location.\"\n    },\n    \"LocationUri\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the location\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-datasync/refs/heads/main/json-schema/location-schema.json
tags:
- AWS
- Data Transfer
- Migration
- Storage
- Automation
- Hybrid Cloud
title: Location
---
