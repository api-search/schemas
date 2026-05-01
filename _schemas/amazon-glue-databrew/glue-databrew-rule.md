---
description: Represents a single data quality requirement that should be validated in the scope of this dataset.
layout: schema
name: Rule
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Disabled
  type: object
- description: ''
  name: CheckExpression
  type: object
- description: ''
  name: SubstitutionMap
  type: object
- description: ''
  name: Threshold
  type: object
- description: ''
  name: ColumnSelectors
  type: object
provider_name: Amazon Glue DataBrew
provider_slug: amazon-glue-databrew
schema_file: json-schema/glue-databrew-rule-schema.json
slug: glue-databrew-rule
source_filename: glue-databrew-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-rule-schema.json\",\n  \"title\": \"Rule\",\n  \"description\": \"Represents a single data quality requirement that should be validated in the scope of this dataset.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleName\"\n        },\n        {\n          \"description\": \"The name of the rule.\"\n        }\n      ]\n    },\n    \"Disabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Disabled\"\n        },\n        {\n          \"description\": \"A value that specifies whether the rule is disabled. Once a rule is disabled, a profile job will not validate it during a job run. Default value is false.\"\n        }\n      ]\n    },\n    \"CheckExpression\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Expression\"\n        },\n        {\n          \"description\": \"<p>The expression which includes column references, condition names followed by variable references, possibly grouped and combined with other conditions. For example, <code>(:col1 starts_with :prefix1 or :col1 starts_with :prefix2) and (:col1 ends_with :suffix1 or :col1 ends_with :suffix2)</code>. Column and value references are substitution variables that should start with the ':' symbol. Depending on the context, substitution variables' values can be either an actual value or a column name. These values are defined in the SubstitutionMap. If a CheckExpression starts with a column reference, then ColumnSelectors in the rule should be null. If ColumnSelectors has been defined, then there should be no column reference in the left side of a condition, for example, <code>is_between :val1 and :val2</code>.</p> <p>For more information, see <a href=\\\
  \"https://docs.aws.amazon.com/databrew/latest/dg/profile.data-quality-available-checks.html\\\">Available checks</a> </p>\"\n        }\n      ]\n    },\n    \"SubstitutionMap\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ValuesMap\"\n        },\n        {\n          \"description\": \"The map of substitution variable names to their values used in a check expression. Variable names should start with a ':' (colon). Variable values can either be actual values or column names. To differentiate between the two, column names should be enclosed in backticks, for example, <code>\\\":col1\\\": \\\"`Column A`\\\".</code> \"\n        }\n      ]\n    },\n    \"Threshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Threshold\"\n        },\n        {\n          \"description\": \"The threshold used with a non-aggregate check expression. Non-aggregate check expressions will be applied to each row in a specific column, and the threshold\
  \ will be used to determine whether the validation succeeds.\"\n        }\n      ]\n    },\n    \"ColumnSelectors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColumnSelectorList\"\n        },\n        {\n          \"description\": \"List of column selectors. Selectors can be used to select columns using a name or regular expression from the dataset. Rule will be applied to selected columns.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"CheckExpression\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue-databrew/refs/heads/main/json-schema/glue-databrew-rule-schema.json
tags:
- Data Analytics
- Data Preparation
- ETL
- Machine Learning
title: Rule
---
