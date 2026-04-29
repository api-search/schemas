---
description: ListChangeSetsRequest schema from Amazon Marketplace API
layout: schema
name: ListChangeSetsRequest
properties_list:
- description: ''
  name: Catalog
  type: object
- description: ''
  name: FilterList
  type: object
- description: ''
  name: Sort
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-list-change-sets-request-schema.json
slug: amazon-marketplace-list-change-sets-request
source_filename: amazon-marketplace-list-change-sets-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-change-sets-request-schema.json\",\n  \"title\": \"ListChangeSetsRequest\",\n  \"description\": \"ListChangeSetsRequest schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Catalog\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Catalog\"\n        },\n        {\n          \"description\": \"The catalog related to the request. Fixed value: <code>AWSMarketplace</code> \"\n        }\n      ]\n    },\n    \"FilterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n          \"description\": \"An array of filter objects.\"\n        }\n      ]\n    },\n    \"Sort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Sort\"\
  \n        },\n        {\n          \"description\": \"An object that contains two attributes, <code>SortBy</code> and <code>SortOrder</code>.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListChangeSetsMaxResultInteger\"\n        },\n        {\n          \"description\": \"The maximum number of results returned by a single call. This value must be provided in the next call to retrieve the next set of results. By default, this value is 20.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token value retrieved from a previous call to access the next page of results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Catalog\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-change-sets-request-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ListChangeSetsRequest
---
