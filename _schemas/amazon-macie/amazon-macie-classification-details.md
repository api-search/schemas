---
description: Provides information about a sensitive data finding and the details of the finding.
layout: schema
name: ClassificationDetails
properties_list:
- description: ''
  name: detailedResultsLocation
  type: object
- description: ''
  name: jobArn
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: originType
  type: object
- description: ''
  name: result
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-classification-details-schema.json
slug: amazon-macie-classification-details
source_filename: amazon-macie-classification-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-details-schema.json\",\n  \"title\": \"ClassificationDetails\",\n  \"description\": \"Provides information about a sensitive data finding and the details of the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"detailedResultsLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The path to the folder or file in Amazon S3 that contains the corresponding sensitive data discovery result for the finding. If a finding applies to a large archive or compressed file, this value is the path to a folder. Otherwise, this value is the path to a file.\"\n        }\n      ]\n    },\n    \"jobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the classification job that produced the finding. This value is null if the origin of the finding (originType) is AUTOMATED_SENSITIVE_DATA_DISCOVERY.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the classification job that produced the finding. This value is null if the origin of the finding (originType) is AUTOMATED_SENSITIVE_DATA_DISCOVERY.\"\n        }\n      ]\n    },\n    \"originType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OriginType\"\n        },\n        {\n          \"description\": \"Specifies how Amazon Macie found the sensitive data that produced the finding. Possible values are: SENSITIVE_DATA_DISCOVERY_JOB, for a classification job; and, AUTOMATED_SENSITIVE_DATA_DISCOVERY, for automated\
  \ sensitive data discovery.\"\n        }\n      ]\n    },\n    \"result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationResult\"\n        },\n        {\n          \"description\": \"The status and other details of the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-classification-details-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ClassificationDetails
---
