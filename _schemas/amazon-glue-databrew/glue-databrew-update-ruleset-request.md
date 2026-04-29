---
description: UpdateRulesetRequest schema from Amazon Glue DataBrew API
layout: schema
name: UpdateRulesetRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Rules
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-update-ruleset-request-schema.json
slug: glue-databrew-update-ruleset-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-ruleset-request-schema.json\",\n  \"title\": \"UpdateRulesetRequest\",\n  \"description\": \"UpdateRulesetRequest schema from Amazon Glue DataBrew API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RulesetDescription\"\n        },\n        {\n          \"description\": \"The description of the ruleset.\"\n        }\n      ]\n    },\n    \"Rules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleList\"\n        },\n        {\n          \"description\": \"A list of rules that are defined with the ruleset. A rule includes one or more checks to be validated on a DataBrew dataset.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Rules\"\n\
  \  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-update-ruleset-request-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: UpdateRulesetRequest
---
