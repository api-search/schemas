---
description: Information about a resource, such as an Amazon S3 bucket or AWS Lambda function, that contains a finding.
layout: schema
name: Resource
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: subResourceId
  type: object
provider_name: Amazon CodeGuru Security
provider_slug: amazon-codeguru-security
schema_file: json-schema/amazon-codeguru-security-resource-schema.json
slug: amazon-codeguru-security-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"Information about a resource, such as an Amazon S3 bucket or AWS Lambda function, that contains a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier for the resource.\"\n        }\n      ]\n    },\n    \"subResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier for a section of the resource, such as an AWS Lambda layer.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-security/refs/heads/main/json-schema/amazon-codeguru-security-resource-schema.json
tags:
- Amazon
- AWS
- Security
- SAST
- Code Analysis
- DevSecOps
- Developer Tools
title: Resource
---
