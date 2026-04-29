---
description: Request message for SetIamPolicy method.
layout: schema
name: SetIamPolicyRequest
properties_list:
- description: A FieldMask specifying which fields of the policy to modify. Only the fields in the mask will be modified.
  name: updateMask
  type: string
provider_name: Google Cloud Platform
provider_slug: google-cloud-platform
schema_file: json-schema/cloud-resource-manager-set-iam-policy-request-schema.json
slug: cloud-resource-manager-set-iam-policy-request
source_filename: cloud-resource-manager-set-iam-policy-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SetIamPolicyRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request message for SetIamPolicy method.\",\n  \"properties\": {\n    \"updateMask\": {\n      \"type\": \"string\",\n      \"description\": \"A FieldMask specifying which fields of the policy to modify. Only the fields in the mask will be modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-platform/refs/heads/main/json-schema/cloud-resource-manager-set-iam-policy-request-schema.json
tags:
- API Management
- Cloud Computing
- Infrastructure
- Platform as a Service
title: SetIamPolicyRequest
---
