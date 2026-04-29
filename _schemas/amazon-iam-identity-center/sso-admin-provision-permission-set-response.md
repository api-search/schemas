---
description: ProvisionPermissionSetResponse schema from AWS IAM Identity Center
layout: schema
name: ProvisionPermissionSetResponse
properties_list:
- description: ''
  name: PermissionSetProvisioningStatus
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-provision-permission-set-response-schema.json
slug: sso-admin-provision-permission-set-response
source_filename: sso-admin-provision-permission-set-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-provision-permission-set-response-schema.json\",\n  \"title\": \"ProvisionPermissionSetResponse\",\n  \"description\": \"ProvisionPermissionSetResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PermissionSetProvisioningStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionSetProvisioningStatus\"\n        },\n        {\n          \"description\": \"The status object for the permission set provisioning operation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-provision-permission-set-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: ProvisionPermissionSetResponse
---
