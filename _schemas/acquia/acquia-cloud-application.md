---
description: application schema from Acquia Cloud API
layout: schema
name: Application
properties_list:
- description: The unique internal ID of the application.
  name: id
  type: integer
- description: The UUID of the application.
  name: uuid
  type: string
- description: The name of the application.
  name: name
  type: string
- description: Hosting details for this application.
  name: hosting
  type: object
- description: ''
  name: subscription
  type: object
- description: ''
  name: organization
  type: object
- description: ''
  name: flags
  type: object
- description: The type of application supported.
  name: type
  type: string
- description: The current application status.
  name: status
  type: string
- description: ''
  name: _links
  type: object
- description: Entities related to the application.
  name: _embedded
  type: object
provider_name: Acquia
provider_slug: acquia
schema_file: json-schema/acquia-cloud-application-schema.json
slug: acquia-cloud-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"application schema from Acquia Cloud API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique internal ID of the application.\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the application.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\"\n    },\n    \"hosting\": {\n      \"type\": \"object\",\n      \"description\": \"Hosting details for this application.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ace\",\n            \"acp\",\n\
  \            \"acsf\",\n            \"free\",\n            \"network\",\n            \"search\",\n            \"unknown\"\n          ],\n          \"description\": \"The hosting type.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The hosting ID.\"\n        }\n      }\n    },\n    \"subscription\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_subscription-stub\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_organization-stub\"\n    },\n    \"flags\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_application-flags\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"drupal\",\n        \"node\",\n        \"ssg\"\n      ],\n      \"description\": \"The type of application supported.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"normal\",\n        \"provisioning\"\
  \n      ],\n      \"description\": \"The current application status.\"\n    },\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_links\"\n    },\n    \"_embedded\": {\n      \"type\": \"object\",\n      \"description\": \"Entities related to the application.\",\n      \"properties\": {\n        \"subscription\": {\n          \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_subscription-stub-embedded\"\n        },\n        \"organization\": {\n          \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_organization-stub-embedded\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Acquia_Cloud_API_Documentation_resource-tag-embedded\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"uuid\",\n    \"name\",\n    \"hosting\",\n    \"subscription\",\n    \"organization\",\n    \"flags\",\n    \"type\",\n\
  \    \"status\",\n    \"_links\",\n    \"_embedded\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acquia/refs/heads/main/json-schema/acquia-cloud-application-schema.json
tags:
- Content
- Experience
title: Application
---
