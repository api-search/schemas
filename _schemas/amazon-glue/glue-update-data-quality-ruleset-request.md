---
description: UpdateDataQualityRulesetRequest schema from Amazon Glue API
layout: schema
name: UpdateDataQualityRulesetRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Ruleset
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-data-quality-ruleset-request-schema.json
slug: glue-update-data-quality-ruleset-request
source_filename: glue-update-data-quality-ruleset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-data-quality-ruleset-request-schema.json\",\n  \"title\": \"UpdateDataQualityRulesetRequest\",\n  \"description\": \"UpdateDataQualityRulesetRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the data quality ruleset.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of the ruleset.\"\n        }\n      ]\n    },\n    \"Ruleset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityRulesetString\"\
  \n        },\n        {\n          \"description\": \"A Data Quality Definition Language (DQDL) ruleset. For more information, see the Glue developer guide.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-data-quality-ruleset-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateDataQualityRulesetRequest
---
