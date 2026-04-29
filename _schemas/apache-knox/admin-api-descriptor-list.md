---
description: List of simple descriptors
layout: schema
name: DescriptorList
properties_list:
- description: ''
  name: descriptors
  type: array
provider_name: Apache Knox
provider_slug: apache-knox
schema_file: json-schema/admin-api-descriptor-list-schema.json
slug: admin-api-descriptor-list
source_filename: admin-api-descriptor-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-descriptor-list-schema.json\",\n  \"title\": \"DescriptorList\",\n  \"description\": \"List of simple descriptors\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"descriptors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Descriptor\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-knox/refs/heads/main/json-schema/admin-api-descriptor-list-schema.json
tags:
- API Gateway
- Authentication
- Hadoop
- Open Source
- Security
- SSO
title: DescriptorList
---
