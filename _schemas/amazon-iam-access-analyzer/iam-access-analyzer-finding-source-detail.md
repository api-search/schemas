---
description: Includes details about how the access that generated the finding is granted. This is populated for Amazon S3 bucket findings.
layout: schema
name: FindingSourceDetail
properties_list:
- description: ''
  name: accessPointArn
  type: object
- description: ''
  name: accessPointAccount
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-finding-source-detail-schema.json
slug: iam-access-analyzer-finding-source-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-finding-source-detail-schema.json\",\n  \"title\": \"FindingSourceDetail\",\n  \"description\": \"Includes details about how the access that generated the finding is granted. This is populated for Amazon S3 bucket findings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessPointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The ARN of the access point that generated the finding. The ARN format depends on whether the ARN represents an access point or a multi-region access point.\"\n        }\n      ]\n    },\n    \"accessPointAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\"\
  : \"The account of the cross-account access point that generated the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-finding-source-detail-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: FindingSourceDetail
---
