---
description: Policy schema from AWS IAM API
layout: schema
name: Policy
properties_list:
- description: The friendly name identifying the policy.
  name: PolicyName
  type: string
- description: The stable and unique string identifying the policy.
  name: PolicyId
  type: string
- description: The Amazon Resource Name (ARN) of the policy.
  name: Arn
  type: string
- description: The path to the policy.
  name: Path
  type: string
- description: The identifier for the version of the policy that is the default.
  name: DefaultVersionId
  type: string
- description: The number of entities the policy is attached to.
  name: AttachmentCount
  type: integer
- description: Specifies whether the policy can be attached.
  name: IsAttachable
  type: boolean
- description: A description of the policy.
  name: Description
  type: string
- description: The date and time when the policy was created.
  name: CreateDate
  type: string
- description: The date and time when the policy was last updated.
  name: UpdateDate
  type: string
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-policy-schema.json
slug: amazon-iam-policy
source_filename: amazon-iam-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-policy-schema.json\",\n  \"title\": \"Policy\",\n  \"description\": \"Policy schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PolicyName\": {\n      \"type\": \"string\",\n      \"description\": \"The friendly name identifying the policy.\"\n    },\n    \"PolicyId\": {\n      \"type\": \"string\",\n      \"description\": \"The stable and unique string identifying the policy.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the policy.\"\n    },\n    \"Path\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the policy.\"\n    },\n    \"DefaultVersionId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the version of the policy that is the default.\"\n \
  \   },\n    \"AttachmentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of entities the policy is attached to.\"\n    },\n    \"IsAttachable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the policy can be attached.\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the policy.\"\n    },\n    \"CreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the policy was created.\"\n    },\n    \"UpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the policy was last updated.\"\n    }\n  },\n  \"required\": [\n    \"PolicyName\",\n    \"PolicyId\",\n    \"Arn\",\n    \"CreateDate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-policy-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity
- Security
title: Policy
---
