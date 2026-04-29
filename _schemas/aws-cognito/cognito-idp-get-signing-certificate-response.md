---
description: Response from Amazon Cognito for a signing certificate request.
layout: schema
name: GetSigningCertificateResponse
properties_list:
- description: ''
  name: Certificate
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-get-signing-certificate-response-schema.json
slug: cognito-idp-get-signing-certificate-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The signing certificate.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Response from Amazon Cognito for a signing certificate request.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-signing-certificate-response-schema.json\",\n  \"title\": \"GetSigningCertificateResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-get-signing-certificate-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: GetSigningCertificateResponse
---
