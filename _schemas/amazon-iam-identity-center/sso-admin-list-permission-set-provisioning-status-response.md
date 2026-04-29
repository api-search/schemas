---
description: ListPermissionSetProvisioningStatusResponse schema from AWS IAM Identity Center
layout: schema
name: ListPermissionSetProvisioningStatusResponse
properties_list:
- description: ''
  name: PermissionSetsProvisioningStatus
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-list-permission-set-provisioning-status-response-schema.json
slug: sso-admin-list-permission-set-provisioning-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-permission-set-provisioning-status-response-schema.json\",\n  \"title\": \"ListPermissionSetProvisioningStatusResponse\",\n  \"description\": \"ListPermissionSetProvisioningStatusResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PermissionSetsProvisioningStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetProvisioningStatusList\"\n        },\n        {\n          \"description\": \"The status object for the permission set provisioning operation.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"The pagination token for the list API. Initially the\
  \ value is null. Use the output of previous API calls to make subsequent calls.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-list-permission-set-provisioning-status-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ListPermissionSetProvisioningStatusResponse
---
