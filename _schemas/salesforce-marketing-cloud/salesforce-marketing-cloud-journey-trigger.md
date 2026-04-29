---
description: Entry trigger configuration for a journey. Defines how contacts enter the journey, such as via API event, scheduled automation, or audience.
layout: schema
name: JourneyTrigger
properties_list:
- description: Unique key for the trigger within the journey
  name: key
  type: string
- description: Display name of the trigger
  name: name
  type: string
- description: Type of trigger
  name: type
  type: string
- description: Key of the event definition associated with this trigger, used for API events
  name: eventDefinitionKey
  type: string
- description: Trigger-specific configuration
  name: configurationArguments
  type: object
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-journey-trigger-schema.json
slug: salesforce-marketing-cloud-journey-trigger
source_filename: salesforce-marketing-cloud-journey-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JourneyTrigger\",\n  \"type\": \"object\",\n  \"description\": \"Entry trigger configuration for a journey. Defines how contacts enter the journey, such as via API event, scheduled automation, or audience.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Unique key for the trigger within the journey\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the trigger\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of trigger\"\n    },\n    \"eventDefinitionKey\": {\n      \"type\": \"string\",\n      \"description\": \"Key of the event definition associated with this trigger, used for API events\"\n    },\n    \"configurationArguments\": {\n      \"type\": \"object\",\n      \"description\": \"Trigger-specific configuration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-journey-trigger-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: JourneyTrigger
---
