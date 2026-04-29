---
description: ListGroupsResponse schema from AWS IAM API
layout: schema
name: ListGroupsResponse
properties_list:
- description: ''
  name: ListGroupsResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-list-groups-response-schema.json
slug: amazon-iam-list-groups-response
source_filename: amazon-iam-list-groups-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-list-groups-response-schema.json\",\n  \"title\": \"ListGroupsResponse\",\n  \"description\": \"ListGroupsResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ListGroupsResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Groups\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Group\"\n          }\n        },\n        \"IsTruncated\": {\n          \"type\": \"boolean\"\n        },\n        \"Marker\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-list-groups-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: ListGroupsResponse
---
