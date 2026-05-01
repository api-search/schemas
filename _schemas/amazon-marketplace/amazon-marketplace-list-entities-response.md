---
description: ListEntitiesResponse schema from Amazon Marketplace API
layout: schema
name: ListEntitiesResponse
properties_list:
- description: ''
  name: EntitySummaryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-list-entities-response-schema.json
slug: amazon-marketplace-list-entities-response
source_filename: amazon-marketplace-list-entities-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-entities-response-schema.json\",\n  \"title\": \"ListEntitiesResponse\",\n  \"description\": \"ListEntitiesResponse schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntitySummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntitySummaryList\"\n        },\n        {\n          \"description\": \" Array of <code>EntitySummary</code> object.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The value of the next token if it exists. Null if there is no more result.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-entities-response-schema.json
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ListEntitiesResponse
---
