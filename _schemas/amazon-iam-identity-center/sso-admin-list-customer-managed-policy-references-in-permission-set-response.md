---
description: ListCustomerManagedPolicyReferencesInPermissionSetResponse schema from AWS IAM Identity Center
layout: schema
name: ListCustomerManagedPolicyReferencesInPermissionSetResponse
properties_list:
- description: ''
  name: CustomerManagedPolicyReferences
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-customer-managed-policy-references-in-permission-set-response-schema.json
slug: sso-admin-list-customer-managed-policy-references-in-permission-set-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-customer-managed-policy-references-in-permission-set-response-schema.json\",\n  \"title\": \"ListCustomerManagedPolicyReferencesInPermissionSetResponse\",\n  \"description\": \"ListCustomerManagedPolicyReferencesInPermissionSetResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomerManagedPolicyReferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerManagedPolicyReferenceList\"\n        },\n        {\n          \"description\": \"Specifies the names and paths of the customer managed policies that you have attached to your permission set.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n\
  \        {\n          \"description\": \"The pagination token for the list API. Initially the value is null. Use the output of previous API calls to make subsequent calls.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-customer-managed-policy-references-in-permission-set-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ListCustomerManagedPolicyReferencesInPermissionSetResponse
---
