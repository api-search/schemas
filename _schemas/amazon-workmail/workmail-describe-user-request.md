---
description: DescribeUserRequest schema from Amazon WorkMail API
layout: schema
name: DescribeUserRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: UserId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-user-request-schema.json
slug: workmail-describe-user-request
source_filename: workmail-describe-user-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"UserId\"\n  ],\n  \"title\": \"DescribeUserRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier for the organization under which the user exists.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkMailIdentifier\"\n        },\n        {\n          \"description\": \"The identifier for the user to be described.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-user-request-schema.json\",\n  \"description\": \"DescribeUserRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-user-request-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeUserRequest
---
