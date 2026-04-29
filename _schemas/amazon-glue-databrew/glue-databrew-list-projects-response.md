---
description: ListProjectsResponse schema from Amazon Glue DataBrew API
layout: schema
name: ListProjectsResponse
properties_list:
- description: ''
  name: Projects
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-list-projects-response-schema.json
slug: glue-databrew-list-projects-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-projects-response-schema.json\",\n  \"title\": \"ListProjectsResponse\",\n  \"description\": \"ListProjectsResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Projects\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectList\"\n        },\n        {\n          \"description\": \"A list of projects that are defined .\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that you can use in a subsequent call to retrieve the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Projects\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-projects-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ListProjectsResponse
---
