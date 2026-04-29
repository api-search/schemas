---
description: An activity within a journey. Activities represent the actions performed on contacts, such as sending emails, waiting, or making decisions.
layout: schema
name: JourneyActivity
properties_list:
- description: Unique key for the activity within the journey
  name: key
  type: string
- description: Display name of the activity
  name: name
  type: string
- description: Type of activity
  name: type
  type: string
- description: Activity-specific configuration
  name: configurationArguments
  type: object
- description: Possible outcomes of the activity leading to next steps
  name: outcomes
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-journey-activity-schema.json
slug: salesforce-marketing-cloud-journey-activity
source_filename: salesforce-marketing-cloud-journey-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JourneyActivity\",\n  \"type\": \"object\",\n  \"description\": \"An activity within a journey. Activities represent the actions performed on contacts, such as sending emails, waiting, or making decisions.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique key for the activity within the journey\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the activity\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of activity\"\n    },\n    \"configurationArguments\": {\n      \"type\": \"object\",\n      \"description\": \"Activity-specific configuration\"\n    },\n    \"outcomes\": {\n      \"type\": \"array\",\n      \"description\": \"Possible outcomes of the activity leading to next steps\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-journey-activity-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: JourneyActivity
---
