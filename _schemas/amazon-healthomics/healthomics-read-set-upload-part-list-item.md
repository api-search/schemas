---
description: The metadata of a single part of a file that was added to a multipart upload. A list of these parts is returned in the response to the ListReadSetUploadParts API.
layout: schema
name: ReadSetUploadPartListItem
properties_list:
- description: ''
  name: partNumber
  type: object
- description: ''
  name: partSize
  type: object
- description: ''
  name: partSource
  type: object
- description: ''
  name: checksum
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: lastUpdatedTime
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-read-set-upload-part-list-item-schema.json
slug: healthomics-read-set-upload-part-list-item
source_filename: healthomics-read-set-upload-part-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-upload-part-list-item-schema.json\",\n  \"title\": \"ReadSetUploadPartListItem\",\n  \"type\": \"object\",\n  \"required\": [\n    \"partNumber\",\n    \"partSize\",\n    \"partSource\",\n    \"checksum\"\n  ],\n  \"properties\": {\n    \"partNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetUploadPartListItemPartNumberInteger\"\n        },\n        {\n          \"description\": \" The number identifying the part in an upload. \"\n        }\n      ]\n    },\n    \"partSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetUploadPartListItemPartSizeLong\"\n        },\n        {\n          \"description\": \" The size of the the part in an upload. \"\n        }\n      ]\n    },\n    \"partSource\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReadSetPartSource\"\n        },\n        {\n          \"description\": \" The origin of the part being direct uploaded. \"\n        }\n      ]\n    },\n    \"checksum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A unique identifier used to confirm that parts are being added to the correct upload. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \" The time stamp for when a direct upload was created. \"\n        }\n      ]\n    },\n    \"lastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyntheticTimestamp_date_time\"\n        },\n        {\n          \"description\": \" The time stamp for the most recent update\
  \ to an uploaded part. \"\n        }\n      ]\n    }\n  },\n  \"description\": \" The metadata of a single part of a file that was added to a multipart upload. A list of these parts is returned in the response to the ListReadSetUploadParts API. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-read-set-upload-part-list-item-schema.json
tags:
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: ReadSetUploadPartListItem
---
