---
description: A named collection of attributes that define a category of contact data, such as Email Addresses or MobileConnect Demographics.
layout: schema
name: AttributeSet
properties_list:
- description: Name of the attribute set
  name: name
  type: string
- description: Collection of attribute value groups
  name: items
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-attribute-set-schema.json
slug: salesforce-marketing-cloud-attribute-set
source_filename: salesforce-marketing-cloud-attribute-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AttributeSet\",\n  \"type\": \"object\",\n  \"description\": \"A named collection of attributes that define a category of contact data, such as Email Addresses or MobileConnect Demographics.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the attribute set\"\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of attribute value groups\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-attribute-set-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: AttributeSet
---
