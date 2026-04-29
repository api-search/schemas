---
description: Budget from LinkedIn API
layout: schema
name: Budget
properties_list:
- description: Budget amount
  name: amount
  type: string
- description: Currency code
  name: currencyCode
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-campaigns-budget-schema.json
slug: linkedin-marketing-campaigns-budget
source_filename: linkedin-marketing-campaigns-budget-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-budget-schema.json\",\n  \"title\": \"Budget\",\n  \"description\": \"Budget from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"string\",\n      \"description\": \"Budget amount\",\n      \"example\": \"1000\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code\",\n      \"example\": \"USD\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-campaigns-budget-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: Budget
---
