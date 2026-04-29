---
description: ListEntitiesRequest schema from Amazon Marketplace API
layout: schema
name: ListEntitiesRequest
properties_list:
- description: ''
  name: Catalog
  type: object
- description: ''
  name: EntityType
  type: object
- description: ''
  name: FilterList
  type: object
- description: ''
  name: Sort
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: OwnershipType
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-list-entities-request-schema.json
slug: amazon-marketplace-list-entities-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-entities-request-schema.json\",\n  \"title\": \"ListEntitiesRequest\",\n  \"description\": \"ListEntitiesRequest schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Catalog\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Catalog\"\n        },\n        {\n          \"description\": \"The catalog related to the request. Fixed value: <code>AWSMarketplace</code> \"\n        }\n      ]\n    },\n    \"EntityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityType\"\n        },\n        {\n          \"description\": \"The type of entities to retrieve.\"\n        }\n      ]\n    },\n    \"FilterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\
  \n        },\n        {\n          \"description\": \"An array of filter objects. Each filter object contains two attributes, <code>filterName</code> and <code>filterValues</code>.\"\n        }\n      ]\n    },\n    \"Sort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Sort\"\n        },\n        {\n          \"description\": \"An object that contains two attributes, <code>SortBy</code> and <code>SortOrder</code>.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The value of the next token, if it exists. Null if there are no more results.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListEntitiesMaxResultInteger\"\n        },\n        {\n          \"description\": \"Specifies the upper limit of the elements on a single page. If a value\
  \ isn't provided, the default value is 20.\"\n        }\n      ]\n    },\n    \"OwnershipType\": {\n      \"$ref\": \"#/components/schemas/OwnershipType\"\n    }\n  },\n  \"required\": [\n    \"Catalog\",\n    \"EntityType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-entities-request-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ListEntitiesRequest
---
