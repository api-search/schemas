---
description: Provide the location for output data from a custom classifier job. This field is mandatory if you are training a native classifier model.
layout: schema
name: DocumentClassifierOutputDataConfig
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: FlywheelStatsS3Prefix
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-document-classifier-output-data-config-schema.json
slug: openapi.yml-document-classifier-output-data-config
source_filename: openapi.yml-document-classifier-output-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-output-data-config-schema.json\",\n  \"title\": \"DocumentClassifierOutputDataConfig\",\n  \"description\": \"Provide the location for output data from a custom classifier job. This field is mandatory if you are training a native classifier model.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"<p>When you use the <code>OutputDataConfig</code> object while creating a custom classifier, you specify the Amazon S3 location where you want to write the confusion matrix and other output files. The URI must be in the same Region as the API endpoint that you are calling. The location is used as the prefix for the actual location\
  \ of this output file.</p> <p>When the custom classifier job is finished, the service creates the output file in a directory specific to the job. The <code>S3Uri</code> field contains the location of the output file, called <code>output.tar.gz</code>. It is a compressed archive that contains the confusion matrix.</p>\"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyId\"\n        },\n        {\n          \"description\": \"<p>ID for the Amazon Web Services Key Management Service (KMS) key that Amazon Comprehend uses to encrypt the output results from an analysis job. The KmsKeyId can be one of the following formats:</p> <ul> <li> <p>KMS Key ID: <code>\\\"1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>Amazon Resource Name (ARN) of a KMS Key: <code>\\\"arn:aws:kms:us-west-2:111122223333:key/1234abcd-12ab-34cd-56ef-1234567890ab\\\"</code> </p> </li> <li> <p>KMS Key Alias: <code>\\\"alias/ExampleAlias\\\
  \"</code> </p> </li> <li> <p>ARN of a KMS Key Alias: <code>\\\"arn:aws:kms:us-west-2:111122223333:alias/ExampleAlias\\\"</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"FlywheelStatsS3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"The Amazon S3 prefix for the data lake location of the flywheel statistics.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-document-classifier-output-data-config-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: DocumentClassifierOutputDataConfig
---
