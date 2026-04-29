---
description: Provides information about the permissions settings of the bucket-level access control list (ACL) for an S3 bucket.
layout: schema
name: AccessControlList
properties_list:
- description: ''
  name: allowsPublicReadAccess
  type: object
- description: ''
  name: allowsPublicWriteAccess
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-access-control-list-schema.json
slug: amazon-macie-access-control-list
source_filename: amazon-macie-access-control-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-access-control-list-schema.json\",\n  \"title\": \"AccessControlList\",\n  \"description\": \"Provides information about the permissions settings of the bucket-level access control list (ACL) for an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowsPublicReadAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the ACL grants the general public with read access permissions for the bucket.\"\n        }\n      ]\n    },\n    \"allowsPublicWriteAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the ACL grants the general public with write access\
  \ permissions for the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-access-control-list-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: AccessControlList
---
