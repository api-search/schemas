---
description: ''
layout: schema
name: field
properties_list:
- description: Field identifier to be used as `fields` input in _Terms-and-Conditions_ endpoints.
  name: field
  type: string
- description: Plain text name of the field.
  name: name
  type: string
- description: Primary Category of field item, such as COUPON_DETAILS or SECURITY_DETAILS.
  name: category
  type: string
- description: The Data Type of the respective field, including - * date * string * integer * double
  name: dataType
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-terms-and-conditions-field-schema.json
slug: factset-terms-and-conditions-field
source_filename: factset-terms-and-conditions-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"field\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"field\": {\n      \"type\": \"string\",\n      \"description\": \"Field identifier to be used as `fields` input in _Terms-and-Conditions_ endpoints.\\n\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text name of the field.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Primary Category of field item, such as COUPON_DETAILS or SECURITY_DETAILS.\"\n    },\n    \"dataType\": {\n      \"type\": \"string\",\n      \"description\": \"The Data Type of the respective field, including -\\n* date\\n* string\\n* integer\\n* double\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-terms-and-conditions-field-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: field
---
