---
description: UpdateInstanceAccessControlAttributeConfigurationRequest schema from AWS IAM Identity Center
layout: schema
name: UpdateInstanceAccessControlAttributeConfigurationRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: InstanceAccessControlAttributeConfiguration
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-update-instance-access-control-attribute-configuration-request-schema.json
slug: sso-admin-update-instance-access-control-attribute-configuration-request
source_filename: sso-admin-update-instance-access-control-attribute-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-update-instance-access-control-attribute-configuration-request-schema.json\",\n  \"title\": \"UpdateInstanceAccessControlAttributeConfigurationRequest\",\n  \"description\": \"UpdateInstanceAccessControlAttributeConfigurationRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed.\"\n        }\n      ]\n    },\n    \"InstanceAccessControlAttributeConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceAccessControlAttributeConfiguration\"\n        },\n\
  \        {\n          \"description\": \"Updates the attributes for your ABAC configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"InstanceAccessControlAttributeConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-update-instance-access-control-attribute-configuration-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: UpdateInstanceAccessControlAttributeConfigurationRequest
---
