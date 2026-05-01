---
description: UpdatePartitionRequest schema from Amazon Glue API
layout: schema
name: UpdatePartitionRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: TableName
  type: object
- description: ''
  name: PartitionValueList
  type: object
- description: ''
  name: PartitionInput
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-partition-request-schema.json
slug: glue-update-partition-request
source_filename: glue-update-partition-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-partition-request-schema.json\",\n  \"title\": \"UpdatePartitionRequest\",\n  \"description\": \"UpdatePartitionRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog where the partition to be updated resides. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the catalog database in which the table in question resides.\"\n        }\n      ]\n \
  \   },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the table in which the partition to be updated is located.\"\n        }\n      ]\n    },\n    \"PartitionValueList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoundedPartitionValueList\"\n        },\n        {\n          \"description\": \"List of partition key values that define the partition to update.\"\n        }\n      ]\n    },\n    \"PartitionInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PartitionInput\"\n        },\n        {\n          \"description\": \"<p>The new partition object to update the partition to.</p> <p>The <code>Values</code> property can't be changed. If you want to change the partition key values for a partition, delete and recreate the partition.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n \
  \   \"DatabaseName\",\n    \"TableName\",\n    \"PartitionValueList\",\n    \"PartitionInput\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-partition-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdatePartitionRequest
---
