---
description: A user account within a Keycloak realm.
layout: schema
name: User
properties_list:
- description: The unique identifier of the user.
  name: id
  type: string
- description: The username.
  name: username
  type: string
- description: The user's first name.
  name: firstName
  type: string
- description: The user's last name.
  name: lastName
  type: string
- description: The user's email address.
  name: email
  type: string
- description: Whether the email has been verified.
  name: emailVerified
  type: boolean
- description: Whether the user account is enabled.
  name: enabled
  type: boolean
- description: The creation timestamp in milliseconds.
  name: createdTimestamp
  type: integer
- description: Custom user attributes.
  name: attributes
  type: object
- description: User credentials configuration.
  name: credentials
  type: array
- description: Actions required on next login.
  name: requiredActions
  type: array
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-keycloak-admin-user-schema.json
slug: red-hat-keycloak-admin-user
source_filename: red-hat-keycloak-admin-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"User\",\n  \"type\": \"object\",\n  \"description\": \"A user account within a Keycloak realm.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's first name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's last name.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The user's email address.\"\n    },\n    \"emailVerified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email has been verified.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is enabled.\"\
  \n    },\n    \"createdTimestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"The creation timestamp in milliseconds.\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom user attributes.\"\n    },\n    \"credentials\": {\n      \"type\": \"array\",\n      \"description\": \"User credentials configuration.\"\n    },\n    \"requiredActions\": {\n      \"type\": \"array\",\n      \"description\": \"Actions required on next login.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-keycloak-admin-user-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: User
---
