---
description: Organization information.
layout: schema
name: Organization
properties_list:
- description: The internal ID of the organization.
  name: id
  type: string
- description: The UUID of the organization.
  name: uuid
  type: string
- description: The name of the organization.
  name: name
  type: string
- description: The number of subscriptions this organization has.
  name: subscriptions_total
  type: integer
- description: The number of administrators this organization has.
  name: admins_total
  type: integer
- description: The number of users this organization has.
  name: users_total
  type: integer
- description: The number of teams this organization has.
  name: teams_total
  type: integer
- description: The number of roles this organization has.
  name: roles_total
  type: integer
- description: ''
  name: owner
  type: object
- description: An array of various flags that indicate functionality for the organization.
  name: flags
  type: object
- description: ''
  name: _links
  type: object
- description: Entities related to the organization.
  name: _embedded
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-organization-schema.json
slug: acquia-cloud-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-organization-schema.json\",\n  \"title\": \"Organization\",\n  \"description\": \"Organization information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The internal ID of the organization.\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The UUID of the organization.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization.\"\n    },\n    \"subscriptions_total\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of subscriptions this organization has.\"\n    },\n    \"admins_total\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of administrators this organization has.\"\n    },\n    \"users_total\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The number of users this organization has.\"\n    },\n    \"teams_total\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of teams this organization has.\"\n    },\n    \"roles_total\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of roles this organization has.\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_user-stub\"\n    },\n    \"flags\": {\n      \"type\": \"object\",\n      \"description\": \"An array of various flags that indicate functionality for the organization.\",\n      \"properties\": {\n        \"federated_authentication\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether the organization supports federated authentication.\"\n        }\n      }\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    },\n    \"_embedded\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Entities related to the organization.\",\n      \"properties\": {\n        \"owner\": {\n          \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_user-stub-embedded\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"uuid\",\n    \"name\",\n    \"subscriptions_total\",\n    \"admins_total\",\n    \"users_total\",\n    \"teams_total\",\n    \"roles_total\",\n    \"owner\",\n    \"flags\",\n    \"_links\",\n    \"_embedded\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-organization-schema.json
tags:
- Content
- Experience
title: Organization
---
