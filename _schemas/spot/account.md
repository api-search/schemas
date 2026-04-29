---
description: A Spot account represents a logical unit within an organization, typically mapped to a cloud provider account or subscription for managing infrastructure resources.
layout: schema
name: Spot Account
properties_list:
- description: The unique identifier of the account.
  name: id
  type: string
- description: The name of the account.
  name: name
  type: string
- description: The identifier of the parent organization.
  name: organizationId
  type: string
- description: The linked cloud provider account identifier.
  name: cloudAccountId
  type: string
- description: The external ID used for cloud provider trust relationships.
  name: providerExternalId
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/account.json
slug: account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/account.json\",\n  \"title\": \"Spot Account\",\n  \"description\": \"A Spot account represents a logical unit within an organization, typically mapped to a cloud provider account or subscription for managing infrastructure resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the account.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the account.\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the parent organization.\"\n    },\n    \"cloudAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The linked cloud provider account identifier.\"\n    },\n    \"providerExternalId\": {\n      \"type\": \"string\",\n \
  \     \"description\": \"The external ID used for cloud provider trust relationships.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/account.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot Account
---
