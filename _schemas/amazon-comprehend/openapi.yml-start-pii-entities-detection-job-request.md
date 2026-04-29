---
description: StartPiiEntitiesDetectionJobRequest schema
layout: schema
name: StartPiiEntitiesDetectionJobRequest
properties_list:
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: Mode
  type: object
- description: ''
  name: RedactionConfig
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-start-pii-entities-detection-job-request-schema.json
slug: openapi.yml-start-pii-entities-detection-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-pii-entities-detection-job-request-schema.json\",\n  \"title\": \"StartPiiEntitiesDetectionJobRequest\",\n  \"description\": \"StartPiiEntitiesDetectionJobRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDataConfig\"\n        },\n        {\n          \"description\": \"The input properties for a PII entities detection job.\"\n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputDataConfig\"\n        },\n        {\n          \"description\": \"Provides con\\ufb01guration parameters for the output of PII entity detection jobs.\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PiiEntitiesDetectionMode\"\n        },\n        {\n          \"description\": \"Specifies whether the output provides the locations (offsets) of PII entities or a file in which PII entities are redacted.\"\n        }\n      ]\n    },\n    \"RedactionConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedactionConfig\"\n        },\n        {\n          \"description\": \"<p>Provides configuration parameters for PII entity redaction.</p> <p>This parameter is required if you set the <code>Mode</code> parameter to <code>ONLY_REDACTION</code>. In that case, you must provide a <code>RedactionConfig</code> definition that includes the <code>PiiEntityTypes</code> parameter.</p>\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource\
  \ Name (ARN) of the IAM role that grants Amazon Comprehend read access to your input data.\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The identifier of the job.\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\": \"The language of the input documents. Currently, English is the only valid language.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestTokenString\"\n        },\n        {\n          \"description\": \"A unique identifier for the request. If you don't set the client request token, Amazon Comprehend generates one.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Tags to associate with the PII entities detection job. A tag is a key-value pair that adds metadata to a resource used by Amazon Comprehend. For example, a tag with \\\"Sales\\\" as the key might be added to a resource to indicate its use by the sales department.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputDataConfig\",\n    \"OutputDataConfig\",\n    \"Mode\",\n    \"DataAccessRoleArn\",\n    \"LanguageCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-pii-entities-detection-job-request-schema.json
tags:
- AWS
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: StartPiiEntitiesDetectionJobRequest
---
