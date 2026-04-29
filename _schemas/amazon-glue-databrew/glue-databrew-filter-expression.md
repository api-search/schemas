---
description: 'Represents a structure for defining parameter conditions. Supported conditions are described here: <a href="https://docs.aws.amazon.com/databrew/latest/dg/datasets.multiple-files.html#conditions.for.dynamic.datasets">Supported conditions for dynamic datasets</a> in the <i>Glue DataBrew Developer Guide</i>.'
layout: schema
name: FilterExpression
properties_list:
- description: ''
  name: Expression
  type: object
- description: ''
  name: ValuesMap
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-filter-expression-schema.json
slug: glue-databrew-filter-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-filter-expression-schema.json\",\n  \"title\": \"FilterExpression\",\n  \"description\": \"Represents a structure for defining parameter conditions. Supported conditions are described here: <a href=\\\"https://docs.aws.amazon.com/databrew/latest/dg/datasets.multiple-files.html#conditions.for.dynamic.datasets\\\">Supported conditions for dynamic datasets</a> in the <i>Glue DataBrew Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Expression\"\n        },\n        {\n          \"description\": \"The expression which includes condition names followed by substitution variables, possibly grouped and combined with other conditions. For example, \\\"(starts_with :prefix1 or\
  \ starts_with :prefix2) and (ends_with :suffix1 or ends_with :suffix2)\\\". Substitution variables should start with ':' symbol.\"\n        }\n      ]\n    },\n    \"ValuesMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValuesMap\"\n        },\n        {\n          \"description\": \"The map of substitution variable names to their values used in this filter expression.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Expression\",\n    \"ValuesMap\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-filter-expression-schema.json
tags:
- AWS
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: FilterExpression
---
