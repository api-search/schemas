---
description: Represents a dataset that can be processed by DataBrew.
layout: schema
name: Dataset
properties_list:
- description: ''
  name: AccountId
  type: object
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
schema_file: json-schema/glue-databrew-dataset-schema.json
slug: glue-databrew-dataset
source_filename: glue-databrew-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"Represents a dataset that can be processed by DataBrew.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account that owns the dataset.\"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who created the dataset.\"\n        }\n      ]\n    },\n    \"CreateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\
  \n        },\n        {\n          \"description\": \"The date and time that the dataset was created.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetName\"\n        },\n        {\n          \"description\": \"The unique name of the dataset.\"\n        }\n      ]\n    },\n    \"Format\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputFormat\"\n        },\n        {\n          \"description\": \"The file format of a dataset that is created from an Amazon S3 file or folder.\"\n        }\n      ]\n    },\n    \"FormatOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FormatOptions\"\n        },\n        {\n          \"description\": \"A set of options that define how DataBrew interprets the data in the dataset.\"\n        }\n      ]\n    },\n    \"Input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Input\"\
  \n        },\n        {\n          \"description\": \"Information on how DataBrew can find the dataset, in either the Glue Data Catalog or Amazon S3.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The last modification date and time of the dataset.\"\n        }\n      ]\n    },\n    \"LastModifiedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastModifiedBy\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the user who last modified the dataset.\"\n        }\n      ]\n    },\n    \"Source\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Source\"\n        },\n        {\n          \"description\": \"The location of the data for the dataset, either Amazon S3 or the Glue Data Catalog.\"\n        }\n      ]\n    },\n    \"PathOptions\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathOptions\"\n        },\n        {\n          \"description\": \"A set of options that defines how DataBrew interprets an Amazon S3 path of the dataset.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Metadata tags that have been applied to the dataset.\"\n        }\n      ]\n    },\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) for the dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Input\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-dataset-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Dataset
---
