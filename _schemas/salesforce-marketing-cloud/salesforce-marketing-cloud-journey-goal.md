---
description: Goal criteria for measuring journey success
layout: schema
name: JourneyGoal
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Criteria expression that defines when the goal is met
  name: metCriteria
  type: string
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-journey-goal-schema.json
slug: salesforce-marketing-cloud-journey-goal
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JourneyGoal\",\n  \"type\": \"object\",\n  \"description\": \"Goal criteria for measuring journey success\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"metCriteria\": {\n      \"type\": \"string\",\n      \"description\": \"Criteria expression that defines when the goal is met\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-journey-goal-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: JourneyGoal
---
