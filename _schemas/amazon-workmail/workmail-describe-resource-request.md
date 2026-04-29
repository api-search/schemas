---
description: DescribeResourceRequest schema from Amazon WorkMail API
layout: schema
name: DescribeResourceRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: ResourceId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-resource-request-schema.json
slug: workmail-describe-resource-request
source_filename: workmail-describe-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"ResourceId\"\n  ],\n  \"title\": \"DescribeResourceRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The identifier associated with the organization for which the resource is described.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier of the resource to be described.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-resource-request-schema.json\",\n  \"description\": \"DescribeResourceRequest schema from Amazon WorkMail\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-resource-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeResourceRequest
---
