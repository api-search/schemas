---
description: ''
layout: schema
name: GetReferenceMetadataResponse
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: arn
  type: object
- description: ''
  name: referenceStoreId
  type: object
- description: ''
  name: md5
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: updateTime
  type: object
- description: ''
  name: files
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-reference-metadata-response-schema.json
slug: healthomics-get-reference-metadata-response
source_filename: healthomics-get-reference-metadata-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-reference-metadata-response-schema.json\",\n  \"title\": \"GetReferenceMetadataResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"arn\",\n    \"referenceStoreId\",\n    \"md5\",\n    \"creationTime\",\n    \"updateTime\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceId\"\n        },\n        {\n          \"description\": \"The reference's ID.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceArn\"\n        },\n        {\n          \"description\": \"The reference's ARN.\"\n        }\n      ]\n    },\n    \"referenceStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStoreId\"\
  \n        },\n        {\n          \"description\": \"The reference's reference store ID.\"\n        }\n      ]\n    },\n    \"md5\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Md5\"\n        },\n        {\n          \"description\": \"The reference's MD5 checksum.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceStatus\"\n        },\n        {\n          \"description\": \"The reference's status.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceName\"\n        },\n        {\n          \"description\": \"The reference's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceDescription\"\n        },\n        {\n          \"description\": \"The reference's description.\"\n        }\n      ]\n    },\n  \
  \  \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the reference was created.\"\n        }\n      ]\n    },\n    \"updateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \"When the reference was updated.\"\n        }\n      ]\n    },\n    \"files\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferenceFiles\"\n        },\n        {\n          \"description\": \"The reference's files.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-reference-metadata-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetReferenceMetadataResponse
---
