---
description: AccessControlAttributeList schema from AWS IAM Identity Center
layout: schema
name: AccessControlAttributeList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-access-control-attribute-list-schema.json
slug: sso-admin-access-control-attribute-list
source_filename: sso-admin-access-control-attribute-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-access-control-attribute-list-schema.json\",\n  \"title\": \"AccessControlAttributeList\",\n  \"description\": \"AccessControlAttributeList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"Key\",\n      \"Value\"\n    ],\n    \"properties\": {\n      \"Key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AccessControlAttributeKey\"\n          },\n          {\n            \"description\": \"The name of the attribute associated with your identities in your identity source. This is used to map a specified attribute in your identity source with an attribute in IAM Identity Center.\"\n          }\n        ]\n      },\n      \"Value\": {\n        \"allOf\": [\n    \
  \      {\n            \"$ref\": \"#/components/schemas/AccessControlAttributeValue\"\n          },\n          {\n            \"description\": \"The value used for mapping a specified attribute to an identity source.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"These are IAM Identity Center identity store attributes that you can configure for use in attributes-based access control (ABAC). You can create permissions policies that determine who can access your AWS resources based upon the configured attribute values. When you enable ABAC and specify <code>AccessControlAttributes</code>, IAM Identity Center passes the attribute values of the authenticated user into IAM for use in policy evaluation.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-access-control-attribute-list-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: AccessControlAttributeList
---
