---
description: ListAccountsForProvisionedPermissionSetRequest schema from AWS IAM Identity Center
layout: schema
name: ListAccountsForProvisionedPermissionSetRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: PermissionSetArn
  type: object
- description: ''
  name: ProvisioningStatus
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-accounts-for-provisioned-permission-set-request-schema.json
slug: sso-admin-list-accounts-for-provisioned-permission-set-request
source_filename: sso-admin-list-accounts-for-provisioned-permission-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-accounts-for-provisioned-permission-set-request-schema.json\",\n  \"title\": \"ListAccountsForProvisionedPermissionSetRequest\",\n  \"description\": \"ListAccountsForProvisionedPermissionSetRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"PermissionSetArn\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetArn\"\n        },\n        {\n          \"description\": \"The ARN of the <a>PermissionSet</a> from which the associated AWS accounts will be listed.\"\n        }\n      ]\n    },\n    \"ProvisioningStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisioningStatus\"\n        },\n        {\n          \"description\": \"The permission set provisioning status for an AWS account.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results to display for the <a>PermissionSet</a>.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"The pagination token for the list API.\
  \ Initially the value is null. Use the output of previous API calls to make subsequent calls.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"PermissionSetArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-accounts-for-provisioned-permission-set-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: ListAccountsForProvisionedPermissionSetRequest
---
