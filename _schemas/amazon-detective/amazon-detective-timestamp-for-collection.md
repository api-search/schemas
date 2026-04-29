---
description: Details on when data collection began for a source package.
layout: schema
name: TimestampForCollection
properties_list:
- description: The data and time when data collection began for a source package.
  name: Timestamp
  type: string
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-timestamp-for-collection-schema.json
slug: amazon-detective-timestamp-for-collection
source_filename: amazon-detective-timestamp-for-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-timestamp-for-collection-schema.json\",\n  \"title\": \"TimestampForCollection\",\n  \"description\": \"Details on when data collection began for a source package.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The data and time when data collection began for a source package.\",\n      \"example\": \"2025-01-15T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-timestamp-for-collection-schema.json
tags:
- AWS
- Forensics
- Investigation
- Security
title: TimestampForCollection
---
