---
description: ListSitesOutput schema from Amazon Outposts
layout: schema
name: ListSitesOutput
properties_list:
- description: ''
  name: Sites
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-list-sites-output-schema.json
slug: openapi-list-sites-output
source_filename: openapi-list-sites-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-sites-output-schema.json\",\n  \"title\": \"ListSitesOutput\",\n  \"description\": \"ListSitesOutput schema from Amazon Outposts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sites\": {\n      \"$ref\": \"#/components/schemas/siteListDefinition\"\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/Token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-list-sites-output-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ListSitesOutput
---
