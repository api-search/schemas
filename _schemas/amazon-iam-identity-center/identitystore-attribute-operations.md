---
description: AttributeOperations schema from AWS IAM Identity Center
layout: schema
name: AttributeOperations
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-attribute-operations-schema.json
slug: identitystore-attribute-operations
source_filename: identitystore-attribute-operations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-attribute-operations-schema.json\",\n  \"title\": \"AttributeOperations\",\n  \"description\": \"AttributeOperations schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"AttributePath\"\n    ],\n    \"properties\": {\n      \"AttributePath\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AttributePath\"\n          },\n          {\n            \"description\": \"A string representation of the path to a given attribute or sub-attribute. Supports JMESPath.\"\n          }\n        ]\n      },\n      \"AttributeValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AttributeValue\"\n          },\n          {\n            \"description\"\
  : \"The value of the attribute. This is a <code>Document</code> type. This type is not supported by Java V1, Go V1, and older versions of the AWS CLI.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"An operation that applies to the requested group. This operation might add, replace, or remove an attribute.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-attribute-operations-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: AttributeOperations
---
