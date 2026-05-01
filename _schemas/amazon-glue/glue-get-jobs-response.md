---
description: GetJobsResponse schema from Amazon Glue API
layout: schema
name: GetJobsResponse
properties_list:
- description: ''
  name: Jobs
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-jobs-response-schema.json
slug: glue-get-jobs-response
source_filename: glue-get-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-jobs-response-schema.json\",\n  \"title\": \"GetJobsResponse\",\n  \"description\": \"GetJobsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobList\"\n        },\n        {\n          \"description\": \"A list of job definitions.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if not all job definitions have yet been returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-jobs-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetJobsResponse
---
