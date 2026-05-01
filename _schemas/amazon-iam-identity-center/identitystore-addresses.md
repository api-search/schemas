---
description: Addresses schema from AWS IAM Identity Center
layout: schema
name: Addresses
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-addresses-schema.json
slug: identitystore-addresses
source_filename: identitystore-addresses-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-addresses-schema.json\",\n  \"title\": \"Addresses\",\n  \"description\": \"Addresses schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"StreetAddress\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"The street of the address.\"\n          }\n        ]\n      },\n      \"Locality\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"A string of the address locality.\"\n          }\n        ]\n      },\n      \"Region\": {\n        \"allOf\": [\n          {\n       \
  \     \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"The region of the address.\"\n          }\n        ]\n      },\n      \"PostalCode\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"The postal code of the address.\"\n          }\n        ]\n      },\n      \"Country\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"The country of the address.\"\n          }\n        ]\n      },\n      \"Formatted\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"A string containing a formatted version of the address for display.\"\n          }\n        ]\n      },\n      \"Type\": {\n   \
  \     \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"A string representing the type of address. For example, \\\"Home.\\\"\"\n          }\n        ]\n      },\n      \"Primary\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveBooleanType\"\n          },\n          {\n            \"description\": \"A Boolean value representing whether this is the primary address for the associated resource.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"The address associated with the specified user.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-addresses-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: Addresses
---
