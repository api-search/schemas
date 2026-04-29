---
description: Specifies the attributes to add to your attribute-based access control (ABAC) configuration.
layout: schema
name: InstanceAccessControlAttributeConfiguration
properties_list:
- description: ''
  name: AccessControlAttributes
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-instance-access-control-attribute-configuration-schema.json
slug: sso-admin-instance-access-control-attribute-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-instance-access-control-attribute-configuration-schema.json\",\n  \"title\": \"InstanceAccessControlAttributeConfiguration\",\n  \"description\": \"Specifies the attributes to add to your attribute-based access control (ABAC) configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessControlAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlAttributeList\"\n        },\n        {\n          \"description\": \"Lists the attributes that are configured for ABAC in the specified IAM Identity Center instance.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccessControlAttributes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-instance-access-control-attribute-configuration-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: InstanceAccessControlAttributeConfiguration
---
