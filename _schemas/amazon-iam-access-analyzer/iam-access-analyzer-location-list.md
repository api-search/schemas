---
description: LocationList schema from AWS IAM Access Analyzer API
layout: schema
name: LocationList
properties_list: []
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-location-list-schema.json
slug: iam-access-analyzer-location-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-location-list-schema.json\",\n  \"title\": \"LocationList\",\n  \"description\": \"LocationList schema from AWS IAM Access Analyzer API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"path\",\n      \"span\"\n    ],\n    \"properties\": {\n      \"path\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/PathElementList\"\n          },\n          {\n            \"description\": \"A path in a policy, represented as a sequence of path elements.\"\n          }\n        ]\n      },\n      \"span\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Span\"\n          },\n          {\n            \"description\": \"A span in a policy.\"\n          }\n        ]\n\
  \      }\n    },\n    \"description\": \"A location in a policy that is represented as a path through the JSON representation and a corresponding span.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-location-list-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: LocationList
---
