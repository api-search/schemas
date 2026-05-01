---
description: The value used for mapping a specified attribute to an identity source. For more information, see <a href="https://docs.aws.amazon.com/singlesignon/latest/userguide/attributemappingsconcept.html">Attribute mappings</a> in the <i>IAM Identity Center User Guide</i>.
layout: schema
name: AccessControlAttributeValue
properties_list:
- description: ''
  name: Source
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-access-control-attribute-value-schema.json
slug: sso-admin-access-control-attribute-value
source_filename: sso-admin-access-control-attribute-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-access-control-attribute-value-schema.json\",\n  \"title\": \"AccessControlAttributeValue\",\n  \"description\": \"The value used for mapping a specified attribute to an identity source. For more information, see <a href=\\\"https://docs.aws.amazon.com/singlesignon/latest/userguide/attributemappingsconcept.html\\\">Attribute mappings</a> in the <i>IAM Identity Center User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControlAttributeValueSourceList\"\n        },\n        {\n          \"description\": \"The identity source to use when mapping a specified attribute to IAM Identity Center.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Source\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-access-control-attribute-value-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: AccessControlAttributeValue
---
