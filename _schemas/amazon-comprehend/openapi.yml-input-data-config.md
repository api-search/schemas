---
description: The input properties for an inference job. The document reader config field applies only to non-text inputs for custom analysis.
layout: schema
name: InputDataConfig
properties_list:
- description: ''
  name: S3Uri
  type: object
- description: ''
  name: InputFormat
  type: object
- description: ''
  name: DocumentReaderConfig
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-input-data-config-schema.json
slug: openapi.yml-input-data-config
source_filename: openapi.yml-input-data-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-input-data-config-schema.json\",\n  \"title\": \"InputDataConfig\",\n  \"description\": \"The input properties for an inference job. The document reader config field applies only to non-text inputs for custom analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Uri\"\n        },\n        {\n          \"description\": \"<p>The Amazon S3 URI for the input data. The URI must be in same Region as the API endpoint that you are calling. The URI can point to a single input file or it can provide the prefix for a collection of data files. </p> <p>For example, if you use the URI <code>S3://bucketName/prefix</code>, if the prefix is a single file, Amazon Comprehend uses that file as input. If more than\
  \ one file begins with the prefix, Amazon Comprehend uses all of them as input.</p>\"\n        }\n      ]\n    },\n    \"InputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFormat\"\n        },\n        {\n          \"description\": \"<p>Specifies how the text in an input file should be processed:</p> <ul> <li> <p> <code>ONE_DOC_PER_FILE</code> - Each file is considered a separate document. Use this option when you are processing large documents, such as newspaper articles or scientific papers.</p> </li> <li> <p> <code>ONE_DOC_PER_LINE</code> - Each line in a file is considered a separate document. Use this option when you are processing many short documents, such as text messages.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"DocumentReaderConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentReaderConfig\"\n        },\n        {\n          \"description\": \"Provides configuration parameters\
  \ to override the default actions for extracting text from PDF documents and image files.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Uri\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-input-data-config-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: InputDataConfig
---
