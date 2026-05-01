---
description: ListSchedulesResponse schema from Amazon Glue DataBrew API
layout: schema
name: ListSchedulesResponse
properties_list:
- description: ''
  name: Schedules
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-list-schedules-response-schema.json
slug: glue-databrew-list-schedules-response
source_filename: glue-databrew-list-schedules-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-schedules-response-schema.json\",\n  \"title\": \"ListSchedulesResponse\",\n  \"description\": \"ListSchedulesResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Schedules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleList\"\n        },\n        {\n          \"description\": \"A list of schedules that are defined.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"A token that you can use in a subsequent call to retrieve the next set of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Schedules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-list-schedules-response-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: ListSchedulesResponse
---
