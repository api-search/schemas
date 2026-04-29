---
description: <p>Provides configuration parameters for the output of inference jobs.</p> <p/>
layout: schema
name: OutputDataConfig
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: KmsKeyId
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-output-data-config-schema.json
slug: openapi.yml-output-data-config
source_filename: openapi.yml-output-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-output-data-config-schema.json\",\n  \"title\": \"OutputDataConfig\",\n  \"description\": \"<p>Provides configuration parameters for the output of inference jobs.</p> <p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"<p>When you use the <code>OutputDataConfig</code> object with asynchronous operations, you specify the Amazon S3 location where you want to write the output data. The URI must be in the same Region as the API endpoint that you are calling. The location is used as the prefix for the actual location of the output file.</p> <p>When the topic detection job is finished, the service creates an output file in a directory specific\
  \ to the job. The <code>S3Uri</code> field contains the location of the output file, called <code>output.tar.gz</code>. It is a compressed archive that contains the ouput of the operation.</p> <p> For a PII entity detection job, the output file is plain text, not a compressed archive. The output file name is the same as the input file, with <code>.out</code> appended at the end. </p>\"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the Amazon Web Services Key Management Service (KMS) key that Amazon Comprehend uses to encrypt the output results from an analysis job. The KmsKeyId can be one of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\"1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\
  \"</code> </p> </li> <li> <p>KMS Key Alias: <code>\\\"alias/ExampleAlias\\\"</code> </p> </li> <li> <p>ARN of a KMS Key Alias: <code>\\\"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-output-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: OutputDataConfig
---
