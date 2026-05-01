---
description: CustomerManagedPolicyReferenceList schema from AWS IAM Identity Center
layout: schema
name: CustomerManagedPolicyReferenceList
properties_list: []
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-customer-managed-policy-reference-list-schema.json
slug: sso-admin-customer-managed-policy-reference-list
source_filename: sso-admin-customer-managed-policy-reference-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-customer-managed-policy-reference-list-schema.json\",\n  \"title\": \"CustomerManagedPolicyReferenceList\",\n  \"description\": \"CustomerManagedPolicyReferenceList schema from AWS IAM Identity Center\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"Name\"\n    ],\n    \"properties\": {\n      \"Name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ManagedPolicyName\"\n          },\n          {\n            \"description\": \"The name of the IAM policy that you have configured in each account where you want to deploy your permission set.\"\n          }\n        ]\n      },\n      \"Path\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ManagedPolicyPath\"\n  \
  \        },\n          {\n            \"description\": \"The path to the IAM policy that you have configured in each account where you want to deploy your permission set. The default is <code>/</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_identifiers.html#identifiers-friendly-names\\\">Friendly names and paths</a> in the <i>IAM User Guide</i>.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Specifies the name and path of a customer managed policy. You must have an IAM policy that matches the name and path in each AWS account where you want to deploy your permission set.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-customer-managed-policy-reference-list-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: CustomerManagedPolicyReferenceList
---
