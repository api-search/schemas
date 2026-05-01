---
description: StartChangeSetRequest schema from Amazon Marketplace API
layout: schema
name: StartChangeSetRequest
properties_list:
- description: ''
  name: Catalog
  type: object
- description: ''
  name: ChangeSet
  type: object
- description: ''
  name: ChangeSetName
  type: object
- description: ''
  name: ClientRequestToken
  type: object
- description: ''
  name: ChangeSetTags
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-start-change-set-request-schema.json
slug: amazon-marketplace-start-change-set-request
source_filename: amazon-marketplace-start-change-set-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-start-change-set-request-schema.json\",\n  \"title\": \"StartChangeSetRequest\",\n  \"description\": \"StartChangeSetRequest schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Catalog\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Catalog\"\n        },\n        {\n          \"description\": \"The catalog related to the request. Fixed value: <code>AWSMarketplace</code> \"\n        }\n      ]\n    },\n    \"ChangeSet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestedChangeList\"\n        },\n        {\n          \"description\": \"Array of <code>change</code> object.\"\n        }\n      ]\n    },\n    \"ChangeSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ChangeSetName\"\n        },\n        {\n          \"description\": \"Optional case sensitive string of up to 100 ASCII characters. The change set name can be used to filter the list of change sets. \"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"A unique token to identify the request to ensure idempotency.\"\n        }\n      ]\n    },\n    \"ChangeSetTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of objects specifying each key name and value for the <code>ChangeSetTags</code> property.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Catalog\",\n    \"ChangeSet\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-start-change-set-request-schema.json
tags:
- Commerce
- ISV
- Marketplace
- Software Catalog
title: StartChangeSetRequest
---
