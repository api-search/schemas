---
description: Contains information on the S3 bucket.
layout: schema
name: S3BucketDetail
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Owner
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: DefaultServerSideEncryption
  type: object
- description: ''
  name: PublicAccess
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-s3-bucket-detail-schema.json
slug: guardduty-s3-bucket-detail
source_filename: guardduty-s3-bucket-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-s3-bucket-detail-schema.json\",\n  \"title\": \"S3BucketDetail\",\n  \"description\": \"Contains information on the S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) of the S3 bucket.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the S3 bucket.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"Describes whether the bucket is a source or destination bucket.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The date and time the bucket was created at.\"\n        }\n      ]\n    },\n    \"Owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Owner\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"owner\"\n          },\n          \"description\": \"The owner of the S3 bucket.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"tags\"\n          },\n          \"description\": \"All tags attached to the S3 bucket\"\n        }\n      ]\n    },\n    \"DefaultServerSideEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultServerSideEncryption\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"defaultServerSideEncryption\"\n          },\n          \"description\": \"Describes the server side encryption method used in the S3 bucket.\"\n        }\n      ]\n    },\n    \"PublicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublicAccess\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publicAccess\"\n          },\n          \"description\": \"Describes the public access policies that apply to the S3 bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-s3-bucket-detail-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: S3BucketDetail
---
