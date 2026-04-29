---
description: A business site with ADT security systems.
layout: schema
name: Site
properties_list:
- description: Unique identifier of the site.
  name: id
  type: string
- description: Name of the business site.
  name: name
  type: string
- description: Physical address.
  name: address
  type: string
- description: Current security status.
  name: status
  type: string
- description: Number of security systems at this site.
  name: systemCount
  type: integer
provider_name: ADT
provider_slug: adt
schema_file: json-schema/business-api-site-schema.json
slug: business-api-site
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-site-schema.json\",\n  \"title\": \"Site\",\n  \"description\": \"A business site with ADT security systems.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the site.\",\n      \"example\": \"site-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the business site.\",\n      \"example\": \"Downtown Office\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Physical address.\",\n      \"example\": \"456 Business Ave, Citytown, CA 90210\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current security status.\",\n      \"enum\": [\n        \"armed\",\n        \"disarmed\",\n        \"alarm\"\n      ],\n\
  \      \"example\": \"armed\"\n    },\n    \"systemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of security systems at this site.\",\n      \"example\": 3\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/business-api-site-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: Site
---
