---
description: <p>The assignment that indicates a principal's limited access to a specified AWS account with a specified permission set.</p> <note> <p>The term <i>principal</i> here refers to a user or group that is defined in IAM Identity Center.</p> </note>
layout: schema
name: AccountAssignment
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: PermissionSetArn
  type: object
- description: ''
  name: PrincipalType
  type: object
- description: ''
  name: PrincipalId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-account-assignment-schema.json
slug: sso-admin-account-assignment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-account-assignment-schema.json\",\n  \"title\": \"AccountAssignment\",\n  \"description\": \"<p>The assignment that indicates a principal's limited access to a specified AWS account with a specified permission set.</p> <note> <p>The term <i>principal</i> here refers to a user or group that is defined in IAM Identity Center.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The identifier of the AWS account.\"\n        }\n      ]\n    },\n    \"PermissionSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetArn\"\n        },\n        {\n          \"description\": \"The\
  \ ARN of the permission set. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"PrincipalType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalType\"\n        },\n        {\n          \"description\": \"The entity type for which the assignment will be created.\"\n        }\n      ]\n    },\n    \"PrincipalId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PrincipalId\"\n        },\n        {\n          \"description\": \"An identifier for an object in IAM Identity Center, such as a user or group. PrincipalIds are GUIDs (For example, f81d4fae-7dec-11d0-a765-00a0c91e6bf6). For more information about PrincipalIds in IAM Identity Center, see the <a href=\\\"/singlesignon/latest/IdentityStoreAPIReference/welcome.html\\\">IAM Identity Center\
  \ Identity Store API Reference</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-account-assignment-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: AccountAssignment
---
