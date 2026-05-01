---
description: <p>Specifies the configuration of the AWS managed or customer managed policy that you want to set as a permissions boundary. Specify either <code>CustomerManagedPolicyReference</code> to use the name and path of a customer managed policy, or <code>ManagedPolicyArn</code> to use the ARN of an AWS managed policy. A permissions boundary represents the maximum permissions that any policy can grant your role. For more information, see <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_boundaries.html">Permissions boundaries for IAM entities</a> in the <i>IAM User Guide</i>.</p> <important> <p>Policies used as permissions boundaries don't provide permissions. You must also attach an IAM policy to the role. To learn how the effective permissions for a role are evaluated, see <a href="https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_evaluation-logic.html">IAM JSON policy evaluation logic</a> in the <i>IAM User Guide</i>.</p> </important>
layout: schema
name: PermissionsBoundary
properties_list:
- description: ''
  name: CustomerManagedPolicyReference
  type: object
- description: ''
  name: ManagedPolicyArn
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-permissions-boundary-schema.json
slug: sso-admin-permissions-boundary
source_filename: sso-admin-permissions-boundary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-permissions-boundary-schema.json\",\n  \"title\": \"PermissionsBoundary\",\n  \"description\": \"<p>Specifies the configuration of the AWS managed or customer managed policy that you want to set as a permissions boundary. Specify either <code>CustomerManagedPolicyReference</code> to use the name and path of a customer managed policy, or <code>ManagedPolicyArn</code> to use the ARN of an AWS managed policy. A permissions boundary represents the maximum permissions that any policy can grant your role. For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_boundaries.html\\\">Permissions boundaries for IAM entities</a> in the <i>IAM User Guide</i>.</p> <important> <p>Policies used as permissions boundaries don't provide permissions. You\
  \ must also attach an IAM policy to the role. To learn how the effective permissions for a role are evaluated, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_evaluation-logic.html\\\">IAM JSON policy evaluation logic</a> in the <i>IAM User Guide</i>.</p> </important>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomerManagedPolicyReference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerManagedPolicyReference\"\n        },\n        {\n          \"description\": \"Specifies the name and path of a customer managed policy. You must have an IAM policy that matches the name and path in each AWS account where you want to deploy your permission set.\"\n        }\n      ]\n    },\n    \"ManagedPolicyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagedPolicyArn\"\n        },\n        {\n          \"description\": \"The AWS managed policy ARN that you want to attach to\
  \ a permission set as a permissions boundary.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-permissions-boundary-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: PermissionsBoundary
---
