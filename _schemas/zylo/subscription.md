---
description: A subscription represents a configured instance of a SaaS application within the Zylo platform. Subscriptions typically have a 1:1 relationship with a given application, though an organization may have multiple subscriptions to the same application.
layout: schema
name: Zylo Subscription
properties_list:
- description: The unique identifier of the subscription.
  name: id
  type: string
- description: The display name of the subscription.
  name: name
  type: string
- description: The ID of the associated application.
  name: applicationId
  type: string
- description: The name of the associated application.
  name: applicationName
  type: string
- description: The current status of the subscription.
  name: status
  type: string
- description: The owner of the subscription.
  name: owner
  type: string
- description: The next renewal date for the subscription.
  name: renewalDate
  type: string
- description: The annual cost of the subscription.
  name: annualCost
  type: number
- description: The total number of licenses for this subscription.
  name: licenseCount
  type: integer
- description: The number of licenses currently in use.
  name: usedLicenseCount
  type: integer
- description: The date and time the subscription was created.
  name: createdAt
  type: string
- description: The date and time the subscription was last updated.
  name: updatedAt
  type: string
- description: Custom fields associated with the subscription.
  name: customFields
  type: object
provider_name: Zylo
provider_slug: zylo
schema_file: json-schema/subscription.json
slug: subscription
source_filename: subscription.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"subscription.json\",\n  \"title\": \"Zylo Subscription\",\n  \"description\": \"A subscription represents a configured instance of a SaaS application within the Zylo platform. Subscriptions typically have a 1:1 relationship with a given application, though an organization may have multiple subscriptions to the same application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the subscription.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the subscription.\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the associated application.\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the associated application.\"\n    },\n    \"status\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The current status of the subscription.\",\n      \"enum\": [\"active\", \"inactive\", \"pending\"]\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The owner of the subscription.\"\n    },\n    \"renewalDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The next renewal date for the subscription.\"\n    },\n    \"annualCost\": {\n      \"type\": \"number\",\n      \"description\": \"The annual cost of the subscription.\"\n    },\n    \"licenseCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of licenses for this subscription.\"\n    },\n    \"usedLicenseCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of licenses currently in use.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the subscription was created.\"\
  \n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the subscription was last updated.\"\n    },\n    \"customFields\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Custom fields associated with the subscription.\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"applicationId\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zylo/refs/heads/main/json-schema/subscription.json
tags:
- Budgets
- SaaS Management
- Spend
title: Zylo Subscription
---
