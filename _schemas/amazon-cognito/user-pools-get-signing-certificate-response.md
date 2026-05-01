---
description: Response from Amazon Cognito for a signing certificate request.
layout: schema
name: GetSigningCertificateResponse
properties_list:
- description: ''
  name: Certificate
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-get-signing-certificate-response-schema.json
slug: user-pools-get-signing-certificate-response
source_filename: user-pools-get-signing-certificate-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-signing-certificate-response-schema.json\",\n  \"title\": \"GetSigningCertificateResponse\",\n  \"description\": \"Response from Amazon Cognito for a signing certificate request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The signing certificate.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-get-signing-certificate-response-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: GetSigningCertificateResponse
---
