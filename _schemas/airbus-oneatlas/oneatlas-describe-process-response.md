---
description: a JSON Object that conforms to the Describe Process Specification v1.0
layout: schema
name: DescribeProcessResponse
properties_list:
- description: ''
  name: _links
  type: object
- description: ''
  name: description
  type: string
- description: ''
  name: family
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: input
  type: object
- description: ''
  name: label
  type: string
- description: ''
  name: version
  type: string
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-describe-process-response-schema.json
slug: oneatlas-describe-process-response
source_filename: oneatlas-describe-process-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-describe-process-response-schema.json\",\n  \"title\": \"DescribeProcessResponse\",\n  \"type\": \"object\",\n  \"description\": \"a JSON Object that conforms to the Describe Process Specification v1.0\",\n  \"properties\": {\n    \"_links\": {\n      \"$ref\": \"#/components/schemas/DescribeProcessLinks\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"family\": {\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"input\": {\n      \"$ref\": \"#/components/schemas/DescribeProcessInput\"\n    },\n    \"label\": {\n      \"type\": \"string\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"label\",\n    \"family\",\n    \"version\",\n    \"input\",\n    \"links\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-describe-process-response-schema.json
tags:
- Imagery
- Satellites
title: DescribeProcessResponse
---
