---
description: CreateCustomEntityTypeRequest schema from Amazon Glue API
layout: schema
name: CreateCustomEntityTypeRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RegexString
  type: object
- description: ''
  name: ContextWords
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-custom-entity-type-request-schema.json
slug: glue-create-custom-entity-type-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-custom-entity-type-request-schema.json\",\n  \"title\": \"CreateCustomEntityTypeRequest\",\n  \"description\": \"CreateCustomEntityTypeRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"A name for the custom pattern that allows it to be retrieved or deleted later. This name must be unique per Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"RegexString\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"A regular expression string that is used for detecting sensitive data in a custom pattern.\"\n\
  \        }\n      ]\n    },\n    \"ContextWords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContextWords\"\n        },\n        {\n          \"description\": \"<p>A list of context words. If none of these context words are found within the vicinity of the regular expression the data will not be detected as sensitive data.</p> <p>If no context words are passed only a regular expression is checked.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RegexString\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-custom-entity-type-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateCustomEntityTypeRequest
---
