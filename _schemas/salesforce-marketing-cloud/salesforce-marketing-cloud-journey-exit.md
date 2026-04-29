---
description: Exit criteria that remove contacts from the journey
layout: schema
name: JourneyExit
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: name
  type: string
- description: Criteria expression that triggers journey exit
  name: criteria
  type: string
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-journey-exit-schema.json
slug: salesforce-marketing-cloud-journey-exit
source_filename: salesforce-marketing-cloud-journey-exit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JourneyExit\",\n  \"type\": \"object\",\n  \"description\": \"Exit criteria that remove contacts from the journey\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"criteria\": {\n      \"type\": \"string\",\n      \"description\": \"Criteria expression that triggers journey exit\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-journey-exit-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: JourneyExit
---
