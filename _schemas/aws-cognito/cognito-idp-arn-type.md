---
description: ArnType schema from Amazon Cognito
layout: schema
name: ArnType
properties_list: []
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-arn-type-schema.json
slug: cognito-idp-arn-type
source_filename: cognito-idp-arn-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"arn:[\\\\w+=/,.@-]+:[\\\\w+=/,.@-]+:([\\\\w+=/,.@-]*)?:[0-9]+:[\\\\w+=/,.@-]+(:[\\\\w+=/,.@-]+)?(:[\\\\w+=/,.@-]+)?\",\n  \"minLength\": 20,\n  \"maxLength\": 2048,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-arn-type-schema.json\",\n  \"title\": \"ArnType\",\n  \"description\": \"ArnType schema from Amazon Cognito\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-arn-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: ArnType
---
