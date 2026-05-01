---
description: The configuration for a custom domain that hosts the sign-up and sign-in webpages for your application.
layout: schema
name: CustomDomainConfigType
properties_list:
- description: ''
  name: CertificateArn
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-custom-domain-config-type-schema.json
slug: user-pools-custom-domain-config-type
source_filename: user-pools-custom-domain-config-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-custom-domain-config-type-schema.json\",\n  \"title\": \"CustomDomainConfigType\",\n  \"description\": \"The configuration for a custom domain that hosts the sign-up and sign-in webpages for your application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnType\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an Certificate Manager SSL certificate. You use this certificate for the subdomain of your custom domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CertificateArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-custom-domain-config-type-schema.json
tags:
- Authentication
- Identity
- OAuth
- User Management
title: CustomDomainConfigType
---
