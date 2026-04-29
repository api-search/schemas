---
description: A JSON Object that conforms to the InputObject as specified in the Describe Process Specification v1.0. It describes the input schema needed in the job creation payload.
layout: schema
name: DescribeProcessInput
properties_list:
- description: ''
  name: definitions
  type: object
- description: ''
  name: properties
  type: object
- description: ''
  name: required
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-describe-process-input-schema.json
slug: oneatlas-describe-process-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-describe-process-input-schema.json\",\n  \"title\": \"DescribeProcessInput\",\n  \"type\": \"object\",\n  \"description\": \"A JSON Object that conforms to the InputObject as specified in the Describe Process Specification v1.0. It describes the input schema needed in the job creation payload.\",\n  \"properties\": {\n    \"definitions\": {\n      \"type\": \"object\"\n    },\n    \"properties\": {\n      \"type\": \"object\"\n    },\n    \"required\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"properties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-describe-process-input-schema.json
tags:
- Imagery
- Satellites
title: DescribeProcessInput
---
