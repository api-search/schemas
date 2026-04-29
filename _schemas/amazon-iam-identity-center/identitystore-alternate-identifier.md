---
description: A unique identifier for a user or group that is not the primary identifier. This value can be an identifier from an external identity provider (IdP) that is associated with the user, the group, or a unique attribute.
layout: schema
name: AlternateIdentifier
properties_list:
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: UniqueAttribute
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-alternate-identifier-schema.json
slug: identitystore-alternate-identifier
source_filename: identitystore-alternate-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-alternate-identifier-schema.json\",\n  \"title\": \"AlternateIdentifier\",\n  \"description\": \"A unique identifier for a user or group that is not the primary identifier. This value can be an identifier from an external identity provider (IdP) that is associated with the user, the group, or a unique attribute.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ExternalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalId\"\n        },\n        {\n          \"description\": \"The identifier issued to this resource by an external identity provider.\"\n        }\n      ]\n    },\n    \"UniqueAttribute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UniqueAttribute\"\n        },\n        {\n          \"\
  description\": \"An entity attribute that's unique to a specific entity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-alternate-identifier-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: AlternateIdentifier
---
