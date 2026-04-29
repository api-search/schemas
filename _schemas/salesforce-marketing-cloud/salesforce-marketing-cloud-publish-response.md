---
description: Response returned when a journey publish operation is initiated
layout: schema
name: PublishResponse
properties_list:
- description: Identifier for tracking the publish operation status
  name: statusId
  type: string
- description: ''
  name: message
  type: string
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-publish-response-schema.json
slug: salesforce-marketing-cloud-publish-response
source_filename: salesforce-marketing-cloud-publish-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response returned when a journey publish operation is initiated\",\n  \"properties\": {\n    \"statusId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier for tracking the publish operation status\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-publish-response-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: PublishResponse
---
