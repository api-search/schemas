---
description: ''
layout: schema
name: RetentionPeriod
properties_list:
- description: The number of units for the retention period.
  name: number
  type: integer
- description: The unit of time that the retention period is measured in.
  name: units
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-audit-retention-period-schema.json
slug: atlassian-confluence-audit-retention-period
source_filename: atlassian-confluence-audit-retention-period-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RetentionPeriod\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"number\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of units for the retention period.\"\n    },\n    \"units\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of time that the retention period is measured in.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-audit-retention-period-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: RetentionPeriod
---
