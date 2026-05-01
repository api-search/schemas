---
description: Additional details about the data set. Different attributes correspond to different data set organizations. The values are populated based on datasetOrg, storageType and backend (Blu Age or Micro Focus).
layout: schema
name: DatasetOrgAttributes
properties_list:
- description: ''
  name: gdg
  type: object
- description: ''
  name: po
  type: object
- description: ''
  name: ps
  type: object
- description: ''
  name: vsam
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-dataset-org-attributes-schema.json
slug: amazon-mainframe-modernization-dataset-org-attributes
source_filename: amazon-mainframe-modernization-dataset-org-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-dataset-org-attributes-schema.json\",\n  \"title\": \"DatasetOrgAttributes\",\n  \"description\": \"Additional details about the data set. Different attributes correspond to different data set organizations. The values are populated based on datasetOrg, storageType and backend (Blu Age or Micro Focus).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gdg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GdgAttributes\"\n        },\n        {\n          \"description\": \"The generation data group of the data set.\"\n        }\n      ]\n    },\n    \"po\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoAttributes\"\n        },\n        {\n          \"description\": \"The details of a PO type\
  \ data set.\"\n        }\n      ]\n    },\n    \"ps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PsAttributes\"\n        },\n        {\n          \"description\": \"The details of a PS type data set.\"\n        }\n      ]\n    },\n    \"vsam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VsamAttributes\"\n        },\n        {\n          \"description\": \"The details of a VSAM data set.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-dataset-org-attributes-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: DatasetOrgAttributes
---
