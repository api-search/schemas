---
description: Response containing all valid values for a parameter.
layout: schema
name: Parameter Values Response
properties_list:
- description: List of valid values for the requested parameter.
  name: param_values
  type: array
provider_name: Agricultural Statistics Service
provider_slug: agricultural-statistics-service
schema_file: json-schema/quickstats-api-param-values-response-schema.json
slug: quickstats-api-param-values-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-param-values-response-schema.json\",\n  \"title\": \"Parameter Values Response\",\n  \"description\": \"Response containing all valid values for a parameter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"param_values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of valid values for the requested parameter.\",\n      \"example\": [\n        \"CORN\",\n        \"SOYBEANS\",\n        \"WHEAT\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agricultural-statistics-service/refs/heads/main/json-schema/quickstats-api-param-values-response-schema.json
tags:
- Agriculture
- Federal Government
- Statistics
- Open Data
- Geospatial
title: Parameter Values Response
---
