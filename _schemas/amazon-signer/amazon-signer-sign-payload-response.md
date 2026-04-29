---
description: SignPayloadResponse schema from AWS Signer API
layout: schema
name: SignPayloadResponse
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: jobOwner
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: signature
  type: object
provider_name: Amazon Signer
provider_slug: amazon-signer
schema_file: json-schema/amazon-signer-sign-payload-response-schema.json
slug: amazon-signer-sign-payload-response
source_filename: amazon-signer-sign-payload-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-sign-payload-response-schema.json\",\n  \"title\": \"SignPayloadResponse\",\n  \"description\": \"SignPayloadResponse schema from AWS Signer API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"Unique identifier of the signing job.\"\n        }\n      ]\n    },\n    \"jobOwner\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{12}$\",\n          \"minLength\": 12,\n          \"maxLength\": 12\n        },\n        {\n          \"description\": \"The AWS account ID of the job owner.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"type\": \"object\",\n          \"additionalProperties\"\
  : {\n            \"$ref\": \"#/components/schemas/String\"\n          }\n        },\n        {\n          \"description\": \"Information including the signing profile ARN and the signing job ID. Clients use metadata to signature records, for example, as annotations added to the signature manifest inside an OCI registry.\"\n        }\n      ]\n    },\n    \"signature\": {\n      \"allOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"description\": \"A cryptographic signature.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-signer/refs/heads/main/json-schema/amazon-signer-sign-payload-response-schema.json
tags:
- AWS
- Code Signing
- IoT
- Lambda
- Security
title: SignPayloadResponse
---
