---
description: ImportModelRequest schema
layout: schema
name: ImportModelRequest
properties_list:
- description: ''
  name: SourceModelArn
  type: object
- description: ''
  name: ModelName
  type: object
- description: ''
  name: VersionName
  type: object
- description: ''
  name: ModelKmsKeyId
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-import-model-request-schema.json
slug: openapi.yml-import-model-request
source_filename: openapi.yml-import-model-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-import-model-request-schema.json\",\n  \"title\": \"ImportModelRequest\",\n  \"description\": \"ImportModelRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceModelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendModelArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom model to import.\"\n        }\n      ]\n    },\n    \"ModelName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArnName\"\n        },\n        {\n          \"description\": \"The name to assign to the custom model that is created in Amazon Comprehend by this import.\"\n        }\n      ]\n    },\n    \"VersionName\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/VersionName\"\n        },\n        {\n          \"description\": \"The version name given to the custom model that is created by this import. Version names can have a maximum of 256 characters. Alphanumeric characters, hyphens (-) and underscores (_) are allowed. The version name must be unique among all models with the same classifier name in the account/Region.\"\n        }\n      ]\n    },\n    \"ModelKmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the KMS key that Amazon Comprehend uses to encrypt trained custom models. The ModelKmsKeyId can be either of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\"1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> </ul>\"\n \
  \       }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend permission to use Amazon Key Management Service (KMS) to encrypt or decrypt the custom model.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Tags to associate with the custom model that is created by this import. A tag is a key-value pair that adds as a metadata to a resource used by Amazon Comprehend. For example, a tag with \\\"Sales\\\" as the key might be added to a resource to indicate its use by the sales department.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SourceModelArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-import-model-request-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: ImportModelRequest
---
