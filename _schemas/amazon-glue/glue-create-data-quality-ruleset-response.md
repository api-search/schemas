---
description: CreateDataQualityRulesetResponse schema from Amazon Glue API
layout: schema
name: CreateDataQualityRulesetResponse
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-data-quality-ruleset-response-schema.json
slug: glue-create-data-quality-ruleset-response
source_filename: glue-create-data-quality-ruleset-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-data-quality-ruleset-response-schema.json\",\n  \"title\": \"CreateDataQualityRulesetResponse\",\n  \"description\": \"CreateDataQualityRulesetResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"A unique name for the data quality ruleset.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-data-quality-ruleset-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateDataQualityRulesetResponse
---
