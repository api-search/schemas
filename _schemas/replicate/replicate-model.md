---
description: A machine learning model hosted on Replicate.
layout: schema
name: Replicate Model
properties_list:
- description: The URL of the model on Replicate.
  name: url
  type: string
- description: The account that owns the model.
  name: owner
  type: string
- description: The model name.
  name: name
  type: string
- description: A description of the model.
  name: description
  type:
  - string
  - 'null'
- description: The visibility of the model.
  name: visibility
  type: string
- description: URL of the model's source code on GitHub.
  name: github_url
  type:
  - string
  - 'null'
- description: URL of the research paper for this model.
  name: paper_url
  type:
  - string
  - 'null'
- description: URL of the model's license.
  name: license_url
  type:
  - string
  - 'null'
- description: How many times this model has been run.
  name: run_count
  type: integer
- description: URL for the model's cover image.
  name: cover_image_url
  type:
  - string
  - 'null'
- description: Example prediction showcasing the model.
  name: default_example
  type:
  - object
  - 'null'
- description: Whether the model is featured on Replicate.
  name: featured
  type: boolean
- description: Tags categorizing the model.
  name: tags
  type: array
- description: ''
  name: latest_version
  type: object
provider_name: Replicate
provider_slug: replicate
schema_file: json-schema/replicate-model-schema.json
slug: replicate-model
source_filename: replicate-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/replicate/json-schema/replicate-model-schema.json\",\n  \"title\": \"Replicate Model\",\n  \"description\": \"A machine learning model hosted on Replicate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the model on Replicate.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The account that owns the model.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The model name.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A description of the model.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"The visibility of the model.\"\n    },\n    \"github_url\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL of the model's source code on GitHub.\"\n    },\n    \"paper_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL of the research paper for this model.\"\n    },\n    \"license_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL of the model's license.\"\n    },\n    \"run_count\": {\n      \"type\": \"integer\",\n      \"description\": \"How many times this model has been run.\"\n    },\n    \"cover_image_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"URL for the model's cover image.\"\n    },\n    \"default_example\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Example prediction showcasing the model.\"\n    },\n    \"featured\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the model is featured on Replicate.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags categorizing the model.\"\n    },\n    \"latest_version\": {\n      \"$ref\": \"#/$defs/ModelVersion\"\n    }\n  },\n  \"required\": [\"owner\", \"name\"],\n  \"$defs\": {\n    \"ModelVersion\": {\n      \"type\": \"object\",\n      \"title\": \"Model Version\",\n      \"description\": \"A specific version of a Replicate model.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the model version.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the version was created.\"\n        },\n        \"cog_version\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The version of Cog used to build this version.\"\
  \n        },\n        \"openapi_schema\": {\n          \"type\": \"object\",\n          \"description\": \"OpenAPI schema describing the model's inputs and outputs.\"\n        }\n      },\n      \"required\": [\"id\", \"created_at\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/replicate/refs/heads/main/json-schema/replicate-model-schema.json
tags:
- Artificial Intelligence
- Machine Learning
- Image Generation
- Language Models
- Model Deployment
title: Replicate Model
---
