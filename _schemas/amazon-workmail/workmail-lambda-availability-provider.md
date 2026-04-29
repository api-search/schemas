---
description: Describes a Lambda based availability provider.
layout: schema
name: LambdaAvailabilityProvider
properties_list:
- description: ''
  name: LambdaArn
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-lambda-availability-provider-schema.json
slug: workmail-lambda-availability-provider
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"LambdaArn\"\n  ],\n  \"properties\": {\n    \"LambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Lambda that acts as the availability provider.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a Lambda based availability provider.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LambdaAvailabilityProvider\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-lambda-availability-provider-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-lambda-availability-provider-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: LambdaAvailabilityProvider
---
