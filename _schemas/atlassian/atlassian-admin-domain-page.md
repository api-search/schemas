---
description: A paginated list of domains.
layout: schema
name: DomainPage
properties_list:
- description: The list of domains.
  name: data
  type: array
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-admin-domain-page-schema.json
slug: atlassian-admin-domain-page
source_filename: atlassian-admin-domain-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DomainPage\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of domains.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of domains.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-admin-domain-page-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: DomainPage
---
