---
description: StartProjectSessionRequest schema from Amazon Glue DataBrew API
layout: schema
name: StartProjectSessionRequest
properties_list:
- description: ''
  name: AssumeControl
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-start-project-session-request-schema.json
slug: glue-databrew-start-project-session-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-start-project-session-request-schema.json\",\n  \"title\": \"StartProjectSessionRequest\",\n  \"description\": \"StartProjectSessionRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AssumeControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssumeControl\"\n        },\n        {\n          \"description\": \"A value that, if true, enables you to take control of a session, even if a different client is currently accessing the project.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-start-project-session-request-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: StartProjectSessionRequest
---
