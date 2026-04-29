---
description: GetResourcePolicyResponse schema from Amazon Marketplace API
layout: schema
name: GetResourcePolicyResponse
properties_list:
- description: ''
  name: Policy
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-get-resource-policy-response-schema.json
slug: amazon-marketplace-get-resource-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-get-resource-policy-response-schema.json\",\n  \"title\": \"GetResourcePolicyResponse\",\n  \"description\": \"GetResourcePolicyResponse schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicyJson\"\n        },\n        {\n          \"description\": \"The policy document to set; formatted in JSON.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-get-resource-policy-response-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: GetResourcePolicyResponse
---
