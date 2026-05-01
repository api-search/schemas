---
description: GetTriggersRequest schema from Amazon Glue API
layout: schema
name: GetTriggersRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: DependentJobName
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-triggers-request-schema.json
slug: glue-get-triggers-request
source_filename: glue-get-triggers-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-triggers-request-schema.json\",\n  \"title\": \"GetTriggersRequest\",\n  \"description\": \"GetTriggersRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"A continuation token, if this is a continuation call.\"\n        }\n      ]\n    },\n    \"DependentJobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the job to retrieve triggers for. The trigger that can start this job is returned, and if there is no such trigger, all triggers are returned.\"\n        }\n      ]\n    },\n    \"MaxResults\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum size of the response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-triggers-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetTriggersRequest
---
