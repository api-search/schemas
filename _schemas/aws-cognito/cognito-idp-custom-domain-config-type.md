---
description: The configuration for a custom domain that hosts the sign-up and sign-in webpages for your application.
layout: schema
name: CustomDomainConfigType
properties_list:
- description: ''
  name: CertificateArn
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-custom-domain-config-type-schema.json
slug: cognito-idp-custom-domain-config-type
source_filename: cognito-idp-custom-domain-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an Certificate Manager SSL certificate. You use this certificate for the subdomain of your custom domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateArn\"\n  ],\n  \"description\": \"The configuration for a custom domain that hosts the sign-up and sign-in webpages for your application.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-custom-domain-config-type-schema.json\",\n  \"title\": \"CustomDomainConfigType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-custom-domain-config-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CustomDomainConfigType
---
