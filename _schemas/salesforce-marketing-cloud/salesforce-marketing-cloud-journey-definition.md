---
description: Specification for creating or updating a journey
layout: schema
name: JourneyDefinition
properties_list:
- description: Customer-defined unique key for the journey
  name: key
  type: string
- description: Display name of the journey
  name: name
  type: string
- description: Description of the journey purpose
  name: description
  type: string
- description: Version of the Journey Builder API (e.g., 1.0)
  name: workflowApiVersion
  type: number
- description: ''
  name: triggers
  type: array
- description: ''
  name: activities
  type: array
- description: ''
  name: goals
  type: array
- description: ''
  name: exits
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-journey-definition-schema.json
slug: salesforce-marketing-cloud-journey-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JourneyDefinition\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating or updating a journey\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-defined unique key for the journey\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the journey\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the journey purpose\"\n    },\n    \"workflowApiVersion\": {\n      \"type\": \"number\",\n      \"description\": \"Version of the Journey Builder API (e.g., 1.0)\"\n    },\n    \"triggers\": {\n      \"type\": \"array\"\n    },\n    \"activities\": {\n      \"type\": \"array\"\n    },\n    \"goals\": {\n      \"type\": \"array\"\n    },\n    \"exits\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-journey-definition-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: JourneyDefinition
---
