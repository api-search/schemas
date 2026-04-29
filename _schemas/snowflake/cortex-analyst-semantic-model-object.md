---
description: Represents a semantic model object
layout: schema
name: SemanticModelObject
properties_list:
- description: The path to a file stored in a Snowflake Stage holding the semantic model yaml. Must be a fully qualified stage url
  name: semantic_model_file
  type: string
- description: The name of the Snowflake native semantic model object
  name: semantic_view
  type: string
- description: A string containing the entire semantic model yaml
  name: inline_semantic_model
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-semantic-model-object-schema.json
slug: cortex-analyst-semantic-model-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SemanticModelObject\",\n  \"type\": \"object\",\n  \"description\": \"Represents a semantic model object\",\n  \"properties\": {\n    \"semantic_model_file\": {\n      \"type\": \"string\",\n      \"description\": \"The path to a file stored in a Snowflake Stage holding the semantic model yaml. Must be a fully qualified stage url\"\n    },\n    \"semantic_view\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Snowflake native semantic model object\"\n    },\n    \"inline_semantic_model\": {\n      \"type\": \"string\",\n      \"description\": \"A string containing the entire semantic model yaml\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-semantic-model-object-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: SemanticModelObject
---
