---
description: Filters schema from AWS IAM Identity Center
layout: schema
name: Filters
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-filters-schema.json
slug: identitystore-filters
source_filename: identitystore-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-filters-schema.json\",\n  \"title\": \"Filters\",\n  \"description\": \"Filters schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"AttributePath\",\n      \"AttributeValue\"\n    ],\n    \"properties\": {\n      \"AttributePath\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AttributePath\"\n          },\n          {\n            \"description\": \"The attribute path that is used to specify which attribute name to search. Length limit is 255 characters. For example, <code>UserName</code> is a valid attribute path for the <code>ListUsers</code> API, and <code>DisplayName</code> is a valid attribute path for the <code>ListGroups</code> API.\"\n          }\n \
  \       ]\n      },\n      \"AttributeValue\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/SensitiveStringType\"\n          },\n          {\n            \"description\": \"Represents the data for an attribute. Each attribute value is described as a name-value pair. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"A query filter used by <code>ListUsers</code> and <code>ListGroups</code>. This filter object provides the attribute name and attribute value to search users or groups.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-filters-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: Filters
---
