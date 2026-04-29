---
description: A single attribute name-value pair within an attribute set
layout: schema
name: AttributeValue
properties_list:
- description: Name of the attribute
  name: name
  type: string
- description: Value of the attribute
  name: value
  type: string
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-attribute-value-schema.json
slug: salesforce-marketing-cloud-attribute-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttributeValue\",\n  \"type\": \"object\",\n  \"description\": \"A single attribute name-value pair within an attribute set\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the attribute\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Value of the attribute\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-attribute-value-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: AttributeValue
---
