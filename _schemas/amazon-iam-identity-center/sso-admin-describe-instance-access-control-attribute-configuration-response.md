---
description: DescribeInstanceAccessControlAttributeConfigurationResponse schema from AWS IAM Identity Center
layout: schema
name: DescribeInstanceAccessControlAttributeConfigurationResponse
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusReason
  type: object
- description: ''
  name: InstanceAccessControlAttributeConfiguration
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-describe-instance-access-control-attribute-configuration-response-schema.json
slug: sso-admin-describe-instance-access-control-attribute-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-describe-instance-access-control-attribute-configuration-response-schema.json\",\n  \"title\": \"DescribeInstanceAccessControlAttributeConfigurationResponse\",\n  \"description\": \"DescribeInstanceAccessControlAttributeConfigurationResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceAccessControlAttributeConfigurationStatus\"\n        },\n        {\n          \"description\": \"The status of the attribute configuration process.\"\n        }\n      ]\n    },\n    \"StatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceAccessControlAttributeConfigurationStatusReason\"\n        },\n        {\n  \
  \        \"description\": \"Provides more details about the current status of the specified attribute.\"\n        }\n      ]\n    },\n    \"InstanceAccessControlAttributeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceAccessControlAttributeConfiguration\"\n        },\n        {\n          \"description\": \"Gets the list of IAM Identity Center identity store attributes that have been added to your ABAC configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-describe-instance-access-control-attribute-configuration-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: DescribeInstanceAccessControlAttributeConfigurationResponse
---
