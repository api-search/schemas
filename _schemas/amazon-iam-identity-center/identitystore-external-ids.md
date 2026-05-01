---
description: ExternalIds schema from AWS IAM Identity Center
layout: schema
name: ExternalIds
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-external-ids-schema.json
slug: identitystore-external-ids
source_filename: identitystore-external-ids-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-external-ids-schema.json\",\n  \"title\": \"ExternalIds\",\n  \"description\": \"ExternalIds schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"Issuer\",\n      \"Id\"\n    ],\n    \"properties\": {\n      \"Issuer\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ExternalIdIssuer\"\n          },\n          {\n            \"description\": \"The issuer for an external identifier.\"\n          }\n        ]\n      },\n      \"Id\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ExternalIdIdentifier\"\n          },\n          {\n            \"description\": \"The identifier issued to this resource by an external identity provider.\"\
  \n          }\n        ]\n      }\n    },\n    \"description\": \"The identifier issued to this resource by an external identity provider.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-external-ids-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: ExternalIds
---
