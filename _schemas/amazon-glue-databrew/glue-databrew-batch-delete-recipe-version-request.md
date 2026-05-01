---
description: BatchDeleteRecipeVersionRequest schema from Amazon Glue DataBrew API
layout: schema
name: BatchDeleteRecipeVersionRequest
properties_list:
- description: ''
  name: RecipeVersions
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-batch-delete-recipe-version-request-schema.json
slug: glue-databrew-batch-delete-recipe-version-request
source_filename: glue-databrew-batch-delete-recipe-version-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-batch-delete-recipe-version-request-schema.json\",\n  \"title\": \"BatchDeleteRecipeVersionRequest\",\n  \"description\": \"BatchDeleteRecipeVersionRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecipeVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeVersionList\"\n        },\n        {\n          \"description\": \"An array of version identifiers, for the recipe versions to be deleted. You can specify numeric versions (<code>X.Y</code>) or <code>LATEST_WORKING</code>. <code>LATEST_PUBLISHED</code> is not supported.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RecipeVersions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-batch-delete-recipe-version-request-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: BatchDeleteRecipeVersionRequest
---
