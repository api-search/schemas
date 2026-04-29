---
description: '<p>A list of errors that can occur when registering partition indexes for an existing table.</p> <p>These errors give the details about why an index registration failed and provide a limited number of partitions in the response, so that you can fix the partitions at fault and try registering the index again. The most common set of errors that can occur are categorized as follows:</p> <ul> <li> <p>EncryptedPartitionError: The partitions are encrypted.</p> </li> <li> <p>InvalidPartitionTypeDataError: The partition value doesn''t match the data type for that partition column.</p> </li> <li> <p>MissingPartitionValueError: The partitions are encrypted.</p> </li> <li> <p>UnsupportedPartitionCharacterError: Characters inside the partition value are not supported. For example: U+0000 , U+0001, U+0002.</p> </li> <li> <p>InternalError: Any error which does not belong to other error codes.</p> </li> </ul>'
layout: schema
name: BackfillError
properties_list:
- description: ''
  name: Code
  type: object
- description: ''
  name: Partitions
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-backfill-error-schema.json
slug: glue-backfill-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-backfill-error-schema.json\",\n  \"title\": \"BackfillError\",\n  \"description\": \"<p>A list of errors that can occur when registering partition indexes for an existing table.</p> <p>These errors give the details about why an index registration failed and provide a limited number of partitions in the response, so that you can fix the partitions at fault and try registering the index again. The most common set of errors that can occur are categorized as follows:</p> <ul> <li> <p>EncryptedPartitionError: The partitions are encrypted.</p> </li> <li> <p>InvalidPartitionTypeDataError: The partition value doesn't match the data type for that partition column.</p> </li> <li> <p>MissingPartitionValueError: The partitions are encrypted.</p> </li> <li> <p>UnsupportedPartitionCharacterError: Characters inside\
  \ the partition value are not supported. For example: U+0000 , U+0001, U+0002.</p> </li> <li> <p>InternalError: Any error which does not belong to other error codes.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackfillErrorCode\"\n        },\n        {\n          \"description\": \"The error code for an error that occurred when registering partition indexes for an existing table.\"\n        }\n      ]\n    },\n    \"Partitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackfillErroredPartitionsList\"\n        },\n        {\n          \"description\": \"A list of a limited number of partitions in the response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-backfill-error-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BackfillError
---
