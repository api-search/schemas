---
description: GetUnfilteredPartitionMetadataResponse schema from Amazon Glue API
layout: schema
name: GetUnfilteredPartitionMetadataResponse
properties_list:
- description: ''
  name: Partition
  type: object
- description: ''
  name: AuthorizedColumns
  type: object
- description: ''
  name: IsRegisteredWithLakeFormation
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-unfiltered-partition-metadata-response-schema.json
slug: glue-get-unfiltered-partition-metadata-response
source_filename: glue-get-unfiltered-partition-metadata-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-partition-metadata-response-schema.json\",\n  \"title\": \"GetUnfilteredPartitionMetadataResponse\",\n  \"description\": \"GetUnfilteredPartitionMetadataResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Partition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Partition\"\n        },\n        {\n          \"description\": \"A Partition object containing the partition metadata.\"\n        }\n      ]\n    },\n    \"AuthorizedColumns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameStringList\"\n        },\n        {\n          \"description\": \"A list of column names that the user has been granted access to.\"\n        }\n      ]\n    },\n    \"IsRegisteredWithLakeFormation\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A Boolean value that indicates whether the partition location is registered with Lake Formation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-partition-metadata-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetUnfilteredPartitionMetadataResponse
---
