---
description: A Spot organization is the top-level entity that contains accounts, users, and policies for managing cloud infrastructure through the Spot platform.
layout: schema
name: Spot Organization
properties_list:
- description: The unique identifier of the organization.
  name: id
  type: string
- description: The name of the organization.
  name: name
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/organization.json
slug: organization
source_filename: organization.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/organization.json\",\n  \"title\": \"Spot Organization\",\n  \"description\": \"A Spot organization is the top-level entity that contains accounts, users, and policies for managing cloud infrastructure through the Spot platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the organization.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/organization.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot Organization
---
