---
description: A key:value pair associated with an Amazon Web Services resource. The key:value pair can be anything you define. Typically, the tag key represents a category (such as "environment") and the tag value represents a specific value within that category (such as "test," "development," or "production"). You can add up to 50 tags to each Amazon Web Services resource.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-tag-schema.json
slug: openapi-tag
source_filename: openapi-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"A key:value pair associated with an Amazon Web Services resource. The key:value pair can be anything you define. Typically, the tag key represents a category (such as \\\"environment\\\") and the tag value represents a specific value within that category (such as \\\"test,\\\" \\\"development,\\\" or \\\"production\\\"). You can add up to 50 tags to each Amazon Web Services resource. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"The part of the key:value pair that defines a tag. You can use a tag key to describe a category of information, such as \\\"customer.\\\" Tag keys\
  \ are case-sensitive.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"The part of the key:value pair that defines a tag. You can use a tag value to describe a specific value within a category, such as \\\"companyA\\\" or \\\"companyB.\\\" Tag values are case-sensitive.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tag-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: Tag
---
