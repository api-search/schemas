---
description: ListChangeSetsResponse schema from Amazon Marketplace API
layout: schema
name: ListChangeSetsResponse
properties_list:
- description: ''
  name: ChangeSetSummaryList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-list-change-sets-response-schema.json
slug: amazon-marketplace-list-change-sets-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-change-sets-response-schema.json\",\n  \"title\": \"ListChangeSetsResponse\",\n  \"description\": \"ListChangeSetsResponse schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeSetSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeSetSummaryList\"\n        },\n        {\n          \"description\": \" Array of <code>ChangeSetSummaryListItem</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The value of the next token, if it exists. Null if there are no more results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-list-change-sets-response-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ListChangeSetsResponse
---
