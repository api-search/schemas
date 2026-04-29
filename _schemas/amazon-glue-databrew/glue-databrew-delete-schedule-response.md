---
description: DeleteScheduleResponse schema from Amazon Glue DataBrew API
layout: schema
name: DeleteScheduleResponse
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-delete-schedule-response-schema.json
slug: glue-databrew-delete-schedule-response
source_filename: glue-databrew-delete-schedule-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-delete-schedule-response-schema.json\",\n  \"title\": \"DeleteScheduleResponse\",\n  \"description\": \"DeleteScheduleResponse schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleName\"\n        },\n        {\n          \"description\": \"The name of the schedule that was deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-delete-schedule-response-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: DeleteScheduleResponse
---
