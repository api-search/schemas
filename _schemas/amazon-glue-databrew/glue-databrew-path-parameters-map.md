---
description: A structure that map names of parameters used in the Amazon S3 path of a dataset to their definitions. A definition includes parameter type and conditions.
layout: schema
name: PathParametersMap
properties_list: []
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-path-parameters-map-schema.json
slug: glue-databrew-path-parameters-map
source_filename: glue-databrew-path-parameters-map-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-path-parameters-map-schema.json\",\n  \"title\": \"PathParametersMap\",\n  \"description\": \"A structure that map names of parameters used in the Amazon S3 path of a dataset to their definitions. A definition includes parameter type and conditions.\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/DatasetParameter\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-path-parameters-map-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: PathParametersMap
---
