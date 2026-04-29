---
description: An object containing <code>FieldField</code>, <code>Type</code>, <code>GroupName</code>, and <code>MatchKey</code>.
layout: schema
name: SchemaInputAttribute
properties_list:
- description: ''
  name: fieldName
  type: object
- description: ''
  name: groupName
  type: object
- description: ''
  name: matchKey
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-schema-input-attribute-schema.json
slug: amazon-entity-resolution-schema-input-attribute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-schema-input-attribute-schema.json\",\n  \"title\": \"SchemaInputAttribute\",\n  \"description\": \"An object containing <code>FieldField</code>, <code>Type</code>, <code>GroupName</code>, and <code>MatchKey</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeName\"\n        },\n        {\n          \"description\": \"A string containing the field name.\"\n        }\n      ]\n    },\n    \"groupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeName\"\n        },\n        {\n          \"description\": \"Instruct Entity Resolution to combine several columns into a unified column with the identical attribute type. For example,\
  \ when working with columns such as first_name, middle_name, and last_name, assigning them a common <code>GroupName</code> will prompt Entity Resolution to concatenate them into a single value.\"\n        }\n      ]\n    },\n    \"matchKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeName\"\n        },\n        {\n          \"description\": \"A key that allows grouping of multiple input attributes into a unified matching group. For example, let's consider a scenario where the source table contains various addresses, such as business_address and shipping_address. By assigning the <code>MatchKey</code> <i>Address</i>' to both attributes, Entity Resolution will match records across these fields to create a consolidated matching group. If no <code>MatchKey</code> is specified for a column, it won't be utilized for matching purposes but will still be included in the output table.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/SchemaAttributeType\"\n        },\n        {\n          \"description\": \"The type of the attribute, selected from a list of values.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-schema-input-attribute-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: SchemaInputAttribute
---
