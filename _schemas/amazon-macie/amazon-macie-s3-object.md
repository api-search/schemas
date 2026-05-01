---
description: Provides information about the S3 object that a finding applies to.
layout: schema
name: S3Object
properties_list:
- description: ''
  name: bucketArn
  type: object
- description: ''
  name: eTag
  type: object
- description: ''
  name: extension
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: lastModified
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: publicAccess
  type: object
- description: ''
  name: serverSideEncryption
  type: object
- description: ''
  name: size
  type: object
- description: ''
  name: storageClass
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: versionId
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-object-schema.json
slug: amazon-macie-s3-object
source_filename: amazon-macie-s3-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-object-schema.json\",\n  \"title\": \"S3Object\",\n  \"description\": \"Provides information about the S3 object that a finding applies to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the bucket that contains the object.\"\n        }\n      ]\n    },\n    \"eTag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The entity tag (ETag) that identifies the affected version of the object. If the object was overwritten or changed after Amazon Macie produced the finding, this value might be different from the\
  \ current ETag for the object.\"\n        }\n      ]\n    },\n    \"extension\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The file name extension of the object. If the object doesn't have a file name extension, this value is \\\"\\\".\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The full key (name) that's assigned to the object.\"\n        }\n      ]\n    },\n    \"lastModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when the object was last modified.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n\
  \        },\n        {\n          \"description\": \"The path to the object, including the full key (name).\"\n        }\n      ]\n    },\n    \"publicAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the object is publicly accessible due to the combination of permissions settings that apply to the object.\"\n        }\n      ]\n    },\n    \"serverSideEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerSideEncryption\"\n        },\n        {\n          \"description\": \"The type of server-side encryption that was used to encrypt the object.\"\n        }\n      ]\n    },\n    \"size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total storage size, in bytes, of the object.\"\n        }\n      ]\n    },\n    \"storageClass\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageClass\"\n        },\n        {\n          \"description\": \"The storage class of the object.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyValuePairList\"\n        },\n        {\n          \"description\": \"The tags that are associated with the object.\"\n        }\n      ]\n    },\n    \"versionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The identifier for the affected version of the object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-object-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3Object
---
