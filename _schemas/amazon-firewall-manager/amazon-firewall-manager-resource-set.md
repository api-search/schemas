---
description: A named collection of AWS resources to include in a Firewall Manager policy.
layout: schema
name: ResourceSet
properties_list:
- description: Unique resource set identifier.
  name: Id
  type: string
- description: Name of the resource set.
  name: Name
  type: string
- description: Optional description.
  name: Description
  type: string
- description: List of AWS resource types in the set.
  name: ResourceTypeList
  type: array
- description: Time the resource set was last updated.
  name: LastUpdateTime
  type: string
- description: Status of the resource set.
  name: ResourceSetStatus
  type: string
provider_name: Amazon Firewall Manager
provider_slug: amazon-firewall-manager
schema_file: json-schema/amazon-firewall-manager-resource-set-schema.json
slug: amazon-firewall-manager-resource-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-resource-set-schema.json\",\n  \"title\": \"ResourceSet\",\n  \"description\": \"A named collection of AWS resources to include in a Firewall Manager policy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique resource set identifier.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the resource set.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional description.\"\n    },\n    \"ResourceTypeList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of AWS resource types in the set.\"\n    },\n    \"LastUpdateTime\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Time the resource set was last updated.\"\n    },\n    \"ResourceSetStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"OUT_OF_ADMIN_SCOPE\"\n      ],\n      \"description\": \"Status of the resource set.\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"ResourceTypeList\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-firewall-manager/refs/heads/main/json-schema/amazon-firewall-manager-resource-set-schema.json
tags:
- AWS
- Compliance
- Firewall
- Network Security
- Security
title: ResourceSet
---
