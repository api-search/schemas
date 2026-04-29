---
description: Provides configuration parameters for the output of PII entity detection jobs.
layout: schema
name: PiiOutputDataConfig
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: KmsKeyId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-pii-output-data-config-schema.json
slug: openapi.yml-pii-output-data-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-pii-output-data-config-schema.json\",\n  \"title\": \"PiiOutputDataConfig\",\n  \"description\": \"Provides configuration parameters for the output of PII entity detection jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"<p>When you use the <code>PiiOutputDataConfig</code> object with asynchronous operations, you specify the Amazon S3 location where you want to write the output data. </p> <p> For a PII entity detection job, the output file is plain text, not a compressed archive. The output file name is the same as the input file, with <code>.out</code> appended at the end. </p>\"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"ID for the Amazon Web Services Key Management Service (KMS) key that Amazon Comprehend uses to encrypt the output results from an analysis job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-pii-output-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: PiiOutputDataConfig
---
