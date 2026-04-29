---
description: ''
layout: schema
name: ContactInformation
properties_list:
- description: ''
  name: emails
  type: array
- description: ''
  name: phones
  type: array
- description: ''
  name: addresses
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/person-contact-information-schema.json
slug: person-contact-information
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContactInformation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"emails\": {\n      \"type\": \"array\"\n    },\n    \"phones\": {\n      \"type\": \"array\"\n    },\n    \"addresses\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/person-contact-information-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: ContactInformation
---
