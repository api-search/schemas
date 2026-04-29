---
description: Details about a file.
layout: schema
name: FileInformation
properties_list:
- description: ''
  name: totalParts
  type: object
- description: ''
  name: partSize
  type: object
- description: ''
  name: contentLength
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-file-information-schema.json
slug: healthomics-file-information
source_filename: healthomics-file-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-file-information-schema.json\",\n  \"title\": \"FileInformation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalParts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformationTotalPartsInteger\"\n        },\n        {\n          \"description\": \"The file's total parts.\"\n        }\n      ]\n    },\n    \"partSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformationPartSizeLong\"\n        },\n        {\n          \"description\": \"The file's part size.\"\n        }\n      ]\n    },\n    \"contentLength\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileInformationContentLengthLong\"\n        },\n        {\n          \"description\": \"The file's content length.\"\
  \n        }\n      ]\n    }\n  },\n  \"description\": \"Details about a file.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-file-information-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: FileInformation
---
