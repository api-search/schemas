---
description: <p>Serverless cluster request.</p>
layout: schema
name: ServerlessRequest
properties_list:
- description: ''
  name: VpcConfigs
  type: object
- description: ''
  name: ClientAuthentication
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-serverless-request-schema.json
slug: msk-api-serverless-request
source_filename: msk-api-serverless-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-serverless-request-schema.json\",\n  \"title\": \"ServerlessRequest\",\n  \"description\": \"\\n            <p>Serverless cluster request.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfVpcConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcConfigs\"\n          },\n          \"description\": \"\\n            <p>The configuration of the Amazon VPCs for the cluster.</p>\"\n        }\n      ]\n    },\n    \"ClientAuthentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerlessClientAuthentication\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientAuthentication\"\n          },\n          \"description\"\
  : \"\\n            <p>Includes all client authentication information.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcConfigs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-serverless-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: ServerlessRequest
---
