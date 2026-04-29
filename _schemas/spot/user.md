---
description: A Spot user represents an individual or programmatic identity with permissions to access and manage resources within a Spot organization.
layout: schema
name: Spot User
properties_list:
- description: The unique identifier of the user.
  name: userId
  type: string
- description: The username of the user.
  name: username
  type: string
- description: The email address of the user.
  name: email
  type: string
- description: The first name of the user.
  name: firstName
  type: string
- description: The last name of the user.
  name: lastName
  type: string
- description: The type of user, either a human user or programmatic API user.
  name: type
  type: string
- description: The role assigned to the user within an account.
  name: role
  type: string
- description: The identifier of the organization the user belongs to.
  name: organizationId
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/user.json
slug: user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/user.json\",\n  \"title\": \"Spot User\",\n  \"description\": \"A Spot user represents an individual or programmatic identity with permissions to access and manage resources within a Spot organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user.\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the user.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the user.\"\
  \n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"user\", \"programmatic\"],\n      \"description\": \"The type of user, either a human user or programmatic API user.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\"admin\", \"viewer\", \"editor\"],\n      \"description\": \"The role assigned to the user within an account.\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the organization the user belongs to.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/user.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot User
---
