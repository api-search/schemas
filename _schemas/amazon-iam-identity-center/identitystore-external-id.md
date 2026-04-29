---
description: The identifier issued to this resource by an external identity provider.
layout: schema
name: ExternalId
properties_list:
- description: ''
  name: Issuer
  type: object
- description: ''
  name: Id
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-external-id-schema.json
slug: identitystore-external-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-external-id-schema.json\",\n  \"title\": \"ExternalId\",\n  \"description\": \"The identifier issued to this resource by an external identity provider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Issuer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalIdIssuer\"\n        },\n        {\n          \"description\": \"The issuer for an external identifier.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalIdIdentifier\"\n        },\n        {\n          \"description\": \"The identifier issued to this resource by an external identity provider.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Issuer\",\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-external-id-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ExternalId
---
