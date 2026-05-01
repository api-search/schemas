---
description: Provides information about a PII entities detection job.
layout: schema
name: PiiEntitiesDetectionJobProperties
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobArn
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: Message
  type: object
- description: ''
  name: SubmitTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: InputDataConfig
  type: object
- description: ''
  name: OutputDataConfig
  type: object
- description: ''
  name: RedactionConfig
  type: object
- description: ''
  name: LanguageCode
  type: object
- description: ''
  name: DataAccessRoleArn
  type: object
- description: ''
  name: Mode
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-pii-entities-detection-job-properties-schema.json
slug: openapi.yml-pii-entities-detection-job-properties
source_filename: openapi.yml-pii-entities-detection-job-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-pii-entities-detection-job-properties-schema.json\",\n  \"title\": \"PiiEntitiesDetectionJobProperties\",\n  \"description\": \"Provides information about a PII entities detection job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The identifier assigned to the PII entities detection job.\"\n        }\n      ]\n    },\n    \"JobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the PII entities detection job. It is a unique, fully qualified identifier for the job. It includes the Amazon Web Services\
  \ account, Amazon Web Services Region, and the job ID. The format of the ARN is as follows:</p> <p> <code>arn:&lt;partition&gt;:comprehend:&lt;region&gt;:&lt;account-id&gt;:pii-entities-detection-job/&lt;job-id&gt;</code> </p> <p>The following is an example job ARN:</p> <p> <code>arn:aws:comprehend:us-west-2:111122223333:pii-entities-detection-job/1234abcd12ab34cd56ef1234567890ab</code> </p>\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name that you assigned the PII entities detection job.\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The current status of the PII entities detection job. If the status is <code>FAILED</code>, the <code>Message</code> field shows the reason for the failure.\"\n     \
  \   }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnyLengthString\"\n        },\n        {\n          \"description\": \"A description of the status of a job.\"\n        }\n      ]\n    },\n    \"SubmitTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the PII entities detection job was submitted for processing.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that the PII entities detection job completed.\"\n        }\n      ]\n    },\n    \"InputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDataConfig\"\n        },\n        {\n          \"description\": \"The input properties for a PII entities detection job.\"\
  \n        }\n      ]\n    },\n    \"OutputDataConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PiiOutputDataConfig\"\n        },\n        {\n          \"description\": \"The output data configuration that you supplied when you created the PII entities detection job.\"\n        }\n      ]\n    },\n    \"RedactionConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedactionConfig\"\n        },\n        {\n          \"description\": \"<p>Provides configuration parameters for PII entity redaction.</p> <p>This parameter is required if you set the <code>Mode</code> parameter to <code>ONLY_REDACTION</code>. In that case, you must provide a <code>RedactionConfig</code> definition that includes the <code>PiiEntityTypes</code> parameter.</p>\"\n        }\n      ]\n    },\n    \"LanguageCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LanguageCode\"\n        },\n        {\n          \"description\"\
  : \"The language code of the input documents\"\n        }\n      ]\n    },\n    \"DataAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants Amazon Comprehend read access to your input data.\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PiiEntitiesDetectionMode\"\n        },\n        {\n          \"description\": \"Specifies whether the output provides the locations (offsets) of PII entities or a file in which PII entities are redacted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-pii-entities-detection-job-properties-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: PiiEntitiesDetectionJobProperties
---
