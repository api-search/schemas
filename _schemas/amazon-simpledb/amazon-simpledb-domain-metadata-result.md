---
description: DomainMetadataResult schema from Amazon SimpleDB API
layout: schema
name: DomainMetadataResult
properties_list:
- description: ''
  name: ItemCount
  type: object
- description: ''
  name: ItemNamesSizeBytes
  type: object
- description: ''
  name: AttributeNameCount
  type: object
- description: ''
  name: AttributeNamesSizeBytes
  type: object
- description: ''
  name: AttributeValueCount
  type: object
- description: ''
  name: AttributeValuesSizeBytes
  type: object
- description: ''
  name: Timestamp
  type: object
provider_name: Amazon SimpleDB
provider_slug: amazon-simpledb
schema_file: json-schema/amazon-simpledb-domain-metadata-result-schema.json
slug: amazon-simpledb-domain-metadata-result
source_filename: amazon-simpledb-domain-metadata-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-domain-metadata-result-schema.json\",\n  \"title\": \"DomainMetadataResult\",\n  \"description\": \"DomainMetadataResult schema from Amazon SimpleDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ItemCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of all items in the domain.\"\n        }\n      ]\n    },\n    \"ItemNamesSizeBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total size of all item names in the domain, in bytes.\"\n        }\n      ]\n    },\n    \"AttributeNameCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\
  \n        },\n        {\n          \"description\": \"The number of unique attribute names in the domain.\"\n        }\n      ]\n    },\n    \"AttributeNamesSizeBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total size of all unique attribute names in the domain, in bytes.\"\n        }\n      ]\n    },\n    \"AttributeValueCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The number of all attribute name/value pairs in the domain.\"\n        }\n      ]\n    },\n    \"AttributeValuesSizeBytes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The total size of all attribute values in the domain, in bytes.\"\n        }\n      ]\n    },\n    \"Timestamp\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"The data and time when metadata was calculated, in Epoch (UNIX) seconds.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simpledb/refs/heads/main/json-schema/amazon-simpledb-domain-metadata-result-schema.json
tags:
- Cloud Storage
- Data Storage
- Database
- NoSQL
title: DomainMetadataResult
---
