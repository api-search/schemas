---
description: DescribePermissionSetProvisioningStatusRequest schema from AWS IAM Identity Center
layout: schema
name: DescribePermissionSetProvisioningStatusRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: ProvisionPermissionSetRequestId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-describe-permission-set-provisioning-status-request-schema.json
slug: sso-admin-describe-permission-set-provisioning-status-request
source_filename: sso-admin-describe-permission-set-provisioning-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-describe-permission-set-provisioning-status-request-schema.json\",\n  \"title\": \"DescribePermissionSetProvisioningStatusRequest\",\n  \"description\": \"DescribePermissionSetProvisioningStatusRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"ProvisionPermissionSetRequestId\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUId\"\n        },\n        {\n          \"description\": \"The identifier that is provided by the <a>ProvisionPermissionSet</a> call to retrieve the current status of the provisioning workflow.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"ProvisionPermissionSetRequestId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-describe-permission-set-provisioning-status-request-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: DescribePermissionSetProvisioningStatusRequest
---
