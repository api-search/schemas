---
description: PutResourcePolicyRequest schema from Amazon Marketplace API
layout: schema
name: PutResourcePolicyRequest
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Policy
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-put-resource-policy-request-schema.json
slug: amazon-marketplace-put-resource-policy-request
source_filename: amazon-marketplace-put-resource-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-put-resource-policy-request-schema.json\",\n  \"title\": \"PutResourcePolicyRequest\",\n  \"description\": \"PutResourcePolicyRequest schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Entity resource you want to associate with a resource policy. \"\n        }\n      ]\n    },\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyJson\"\n        },\n        {\n          \"description\": \"The policy document to set; formatted in JSON.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"\
  ResourceArn\",\n    \"Policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-put-resource-policy-request-schema.json
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
title: PutResourcePolicyRequest
---
