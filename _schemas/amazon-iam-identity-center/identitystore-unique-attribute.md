---
description: An entity attribute that's unique to a specific entity.
layout: schema
name: UniqueAttribute
properties_list:
- description: ''
  name: AttributePath
  type: object
- description: ''
  name: AttributeValue
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-unique-attribute-schema.json
slug: identitystore-unique-attribute
source_filename: identitystore-unique-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-unique-attribute-schema.json\",\n  \"title\": \"UniqueAttribute\",\n  \"description\": \"An entity attribute that's unique to a specific entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AttributePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributePath\"\n        },\n        {\n          \"description\": \"A string representation of the path to a given attribute or sub-attribute. Supports JMESPath.\"\n        }\n      ]\n    },\n    \"AttributeValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeValue\"\n        },\n        {\n          \"description\": \"The value of the attribute. This is a <code>Document</code> type. This type is not supported by Java V1, Go V1, and older versions\
  \ of the AWS CLI.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AttributePath\",\n    \"AttributeValue\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-unique-attribute-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: UniqueAttribute
---
