---
description: Represents how metadata stored in the Glue Data Catalog is defined in a DataBrew dataset.
layout: schema
name: DataCatalogInputDefinition
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
  name: TempDirectory
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-data-catalog-input-definition-schema.json
slug: glue-databrew-data-catalog-input-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-data-catalog-input-definition-schema.json\",\n  \"title\": \"DataCatalogInputDefinition\",\n  \"description\": \"Represents how metadata stored in the Glue Data Catalog is defined in a DataBrew dataset. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogId\"\n        },\n        {\n          \"description\": \"The unique identifier of the Amazon Web Services account that holds the Data Catalog that stores the data.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatabaseName\"\n        },\n        {\n          \"description\": \"The name of a database in the Data Catalog.\"\n        }\n      ]\n    },\n\
  \    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableName\"\n        },\n        {\n          \"description\": \"The name of a database table in the Data Catalog. This table corresponds to a DataBrew dataset.\"\n        }\n      ]\n    },\n    \"TempDirectory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"Represents an Amazon location where DataBrew can store intermediate results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-data-catalog-input-definition-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DataCatalogInputDefinition
---
