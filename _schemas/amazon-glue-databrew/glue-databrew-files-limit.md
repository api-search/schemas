---
description: Represents a limit imposed on number of Amazon S3 files that should be selected for a dataset from a connected Amazon S3 path.
layout: schema
name: FilesLimit
properties_list:
- description: ''
  name: MaxFiles
  type: object
- description: ''
  name: OrderedBy
  type: object
- description: ''
  name: Order
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-files-limit-schema.json
slug: glue-databrew-files-limit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-files-limit-schema.json\",\n  \"title\": \"FilesLimit\",\n  \"description\": \"Represents a limit imposed on number of Amazon S3 files that should be selected for a dataset from a connected Amazon S3 path.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxFiles\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxFiles\"\n        },\n        {\n          \"description\": \"The number of Amazon S3 files to select.\"\n        }\n      ]\n    },\n    \"OrderedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrderedBy\"\n        },\n        {\n          \"description\": \"A criteria to use for Amazon S3 files sorting before their selection. By default uses LAST_MODIFIED_DATE as a sorting criteria. Currently it's the\
  \ only allowed value.\"\n        }\n      ]\n    },\n    \"Order\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Order\"\n        },\n        {\n          \"description\": \"A criteria to use for Amazon S3 files sorting before their selection. By default uses DESCENDING order, i.e. most recent files are selected first. Another possible value is ASCENDING.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"MaxFiles\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-files-limit-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: FilesLimit
---
