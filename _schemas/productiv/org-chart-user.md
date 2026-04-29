---
description: Represents a user entry in the organizational chart published to the Productiv platform.
layout: schema
name: OrgChartUser
properties_list:
- description: The email address of the user.
  name: email
  type: string
- description: First name of the user.
  name: firstName
  type: string
- description: Last name of the user.
  name: lastName
  type: string
- description: The email address of the user's manager.
  name: managerEmail
  type: string
- description: The department of the user.
  name: department
  type: string
- description: The job title of the user.
  name: title
  type: string
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/org-chart-user.json
slug: org-chart-user
source_filename: org-chart-user.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"org-chart-user.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrgChartUser\",\n  \"description\": \"Represents a user entry in the organizational chart published to the Productiv platform.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"email\"\n  ],\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the user.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the user.\"\n    },\n    \"managerEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user's manager.\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"The department of the user.\"\n    },\n    \"title\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The job title of the user.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/org-chart-user.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: OrgChartUser
---
