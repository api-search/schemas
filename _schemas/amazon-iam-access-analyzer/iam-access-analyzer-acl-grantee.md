---
description: You specify each grantee as a type-value pair using one of these types. You can specify only one type of grantee. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutBucketAcl.html">PutBucketAcl</a>.
layout: schema
name: AclGrantee
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: uri
  type: object
provider_name: Amazon IAM Access Analyzer
provider_slug: amazon-iam-access-analyzer
schema_file: json-schema/iam-access-analyzer-acl-grantee-schema.json
slug: iam-access-analyzer-acl-grantee
source_filename: iam-access-analyzer-acl-grantee-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-acl-grantee-schema.json\",\n  \"title\": \"AclGrantee\",\n  \"description\": \"You specify each grantee as a type-value pair using one of these types. You can specify only one type of grantee. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutBucketAcl.html\\\">PutBucketAcl</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AclCanonicalId\"\n        },\n        {\n          \"description\": \"The value specified is the canonical user ID of an Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AclUri\"\n        },\n        {\n          \"description\"\
  : \"Used for granting permissions to a predefined group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-access-analyzer/refs/heads/main/json-schema/iam-access-analyzer-acl-grantee-schema.json
tags:
- Access Control
- AWS
- Compliance
- IAM
- Policy Management
- Security
title: AclGrantee
---
