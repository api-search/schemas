---
description: Represents a user provisioned to an application in the Productiv platform.
layout: schema
name: ProvisionedUser
properties_list:
- description: The email address of the user.
  name: email
  type: string
- description: The first name of the user.
  name: firstName
  type: string
- description: The last name of the user.
  name: lastName
  type: string
- description: The role of the user in the application.
  name: role
  type: string
provider_name: Productiv
provider_slug: productiv
schema_file: json-schema/provisioned-user.json
slug: provisioned-user
source_filename: provisioned-user.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"provisioned-user.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProvisionedUser\",\n  \"description\": \"Represents a user provisioned to an application in the Productiv platform.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"email\"\n  ],\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the user.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the user.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role of the user in the application.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/productiv/refs/heads/main/json-schema/provisioned-user.json
tags:
- Application Portfolio
- Provisioning
- SaaS Management
- Spend Management
- Usage Analytics
title: ProvisionedUser
---
