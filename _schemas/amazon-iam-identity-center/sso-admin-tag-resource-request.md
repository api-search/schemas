---
description: TagResourceRequest schema from AWS IAM Identity Center
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: InstanceArn
  type: object
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/sso-admin-tag-resource-request-schema.json
slug: sso-admin-tag-resource-request
source_filename: sso-admin-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM Identity Center instance under which the operation will be executed. For more information about ARNs, see <a href=\\\"/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs) and AWS Service Namespaces</a> in the <i>AWS General Reference</i>.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaggableResourceArn\"\
  \n        },\n        {\n          \"description\": \"The ARN of the resource with the tags to be listed.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A set of key-value pairs that are used to manage the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InstanceArn\",\n    \"ResourceArn\",\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/sso-admin-tag-resource-request-schema.json
tags:
- Access Control
- Authentication
- Identity Management
- Single Sign-On
title: TagResourceRequest
---
