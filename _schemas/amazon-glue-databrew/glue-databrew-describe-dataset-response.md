---
description: DescribeDatasetResponse schema from Amazon Glue DataBrew API
layout: schema
name: DescribeDatasetResponse
properties_list:
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: CreateDate
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Format
  type: object
- description: ''
  name: FormatOptions
  type: object
- description: ''
  name: Input
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: LastModifiedBy
  type: object
- description: ''
  name: Source
  type: object
- description: ''
  name: PathOptions
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ResourceArn
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-describe-dataset-response-schema.json
slug: glue-databrew-describe-dataset-response
source_filename: glue-databrew-describe-dataset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-dataset-response-schema.json\",\n  \"title\": \"DescribeDatasetResponse\",\n  \"description\": \"DescribeDatasetResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user who created the dataset.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the dataset was created.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\
  \n        },\n        {\n          \"description\": \"The name of the dataset.\"\n        }\n      ]\n    },\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFormat\"\n        },\n        {\n          \"description\": \"The file format of a dataset that is created from an Amazon S3 file or folder.\"\n        }\n      ]\n    },\n    \"FormatOptions\": {\n      \"$ref\": \"#/components/schemas/FormatOptions\"\n    },\n    \"Input\": {\n      \"$ref\": \"#/components/schemas/Input\"\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The date and time that the dataset was last modified.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The identifier (user name) of the user\
  \ who last modified the dataset.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Source\"\n        },\n        {\n          \"description\": \"The location of the data for this dataset, Amazon S3 or the Glue Data Catalog.\"\n        }\n      ]\n    },\n    \"PathOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathOptions\"\n        },\n        {\n          \"description\": \"A set of options that defines how DataBrew interprets an Amazon S3 path of the dataset.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags associated with this dataset.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The\
  \ Amazon Resource Name (ARN) of the dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Input\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-describe-dataset-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DescribeDatasetResponse
---
