---
description: GetUnfilteredPartitionsMetadataResponse schema from Amazon Glue API
layout: schema
name: GetUnfilteredPartitionsMetadataResponse
properties_list:
- description: ''
  name: UnfilteredPartitions
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-unfiltered-partitions-metadata-response-schema.json
slug: glue-get-unfiltered-partitions-metadata-response
source_filename: glue-get-unfiltered-partitions-metadata-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-partitions-metadata-response-schema.json\",\n  \"title\": \"GetUnfilteredPartitionsMetadataResponse\",\n  \"description\": \"GetUnfilteredPartitionsMetadataResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UnfilteredPartitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnfilteredPartitionList\"\n        },\n        {\n          \"description\": \"A list of requested partitions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list of partitions does not include the last one.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-unfiltered-partitions-metadata-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetUnfilteredPartitionsMetadataResponse
---
