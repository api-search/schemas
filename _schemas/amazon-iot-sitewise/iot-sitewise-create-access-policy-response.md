---
description: CreateAccessPolicyResponse schema
layout: schema
name: CreateAccessPolicyResponse
properties_list:
- description: ''
  name: accessPolicyId
  type: object
- description: ''
  name: accessPolicyArn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-create-access-policy-response-schema.json
slug: iot-sitewise-create-access-policy-response
source_filename: iot-sitewise-create-access-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-access-policy-response-schema.json\",\n  \"title\": \"CreateAccessPolicyResponse\",\n  \"description\": \"CreateAccessPolicyResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPolicyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the access policy.\"\n        }\n      ]\n    },\n    \"accessPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the access policy, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:access-policy/${AccessPolicyId}</code>\
  \ </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accessPolicyId\",\n    \"accessPolicyArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-create-access-policy-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: CreateAccessPolicyResponse
---
