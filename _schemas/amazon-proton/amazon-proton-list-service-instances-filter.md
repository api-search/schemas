---
description: A filtering criterion to scope down the result list of the <a>ListServiceInstances</a> action.
layout: schema
name: ListServiceInstancesFilter
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-service-instances-filter-schema.json
slug: amazon-proton-list-service-instances-filter
source_filename: amazon-proton-list-service-instances-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instances-filter-schema.json\",\n  \"title\": \"ListServiceInstancesFilter\",\n  \"description\": \"A filtering criterion to scope down the result list of the <a>ListServiceInstances</a> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListServiceInstancesFilterBy\"\n        },\n        {\n          \"description\": \"The name of a filtering criterion.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListServiceInstancesFilterValue\"\n        },\n        {\n          \"description\": \"<p>A value to filter by.</p> <p>With the date/time keys (<code>*At{Before,After}</code>), the value is a valid <a href=\\\"\
  https://datatracker.ietf.org/doc/html/rfc3339.html\\\">RFC 3339</a> string with no UTC offset and with an optional fractional precision (for example, <code>1985-04-12T23:20:50.52Z</code>).</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-service-instances-filter-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListServiceInstancesFilter
---
