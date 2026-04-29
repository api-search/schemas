---
description: CreateDataQualityRulesetRequest schema from Amazon Glue API
layout: schema
name: CreateDataQualityRulesetRequest
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
- description: ''
  name: Tags
  type: object
- description: ''
  name: TargetTable
  type: object
- description: ''
  name: ClientToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-data-quality-ruleset-request-schema.json
slug: glue-create-data-quality-ruleset-request
source_filename: glue-create-data-quality-ruleset-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-data-quality-ruleset-request-schema.json\",\n  \"title\": \"CreateDataQualityRulesetRequest\",\n  \"description\": \"CreateDataQualityRulesetRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"A unique name for the data quality ruleset.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of the data quality ruleset.\"\n        }\n      ]\n    },\n    \"Ruleset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityRulesetString\"\
  \n        },\n        {\n          \"description\": \"A Data Quality Definition Language (DQDL) ruleset. For more information, see the Glue developer guide.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"A list of tags applied to the data quality ruleset.\"\n        }\n      ]\n    },\n    \"TargetTable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityTargetTable\"\n        },\n        {\n          \"description\": \"A target table associated with the data quality ruleset.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"Used for idempotency and is recommended to be set to a random ID (such as a UUID) to avoid creating or starting multiple instances of the same resource.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Ruleset\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-data-quality-ruleset-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateDataQualityRulesetRequest
---
