---
description: A named list of seed URLs.
layout: schema
name: SeedList
properties_list:
- description: The seed list identifier.
  name: id
  type: integer
- description: A human-readable name for this seed list.
  name: name
  type: string
- description: The HDFS path where the seed file is stored. Populated after creation.
  name: seedFilePath
  type: string
- description: The collection of seed URLs in this list.
  name: seedUrls
  type: array
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-seed-list-schema.json
slug: apache-nutch-seed-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-seed-list-schema.json\",\n  \"title\": \"SeedList\",\n  \"description\": \"A named list of seed URLs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"minimum\": 0,\n      \"maximum\": 9007199254740991,\n      \"description\": \"The seed list identifier.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for this seed list.\"\n    },\n    \"seedFilePath\": {\n      \"type\": \"string\",\n      \"description\": \"The HDFS path where the seed file is stored. Populated after creation.\",\n      \"readOnly\": true\n    },\n    \"seedUrls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\"\
  : \"A single seed URL entry.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"minimum\": 0,\n            \"maximum\": 9007199254740991,\n            \"description\": \"The seed URL identifier.\",\n            \"readOnly\": true\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"description\": \"The seed URL.\"\n          }\n        },\n        \"example\": {\n          \"url\": \"https://example.com\"\n        }\n      },\n      \"description\": \"The collection of seed URLs in this list.\"\n    }\n  },\n  \"required\": [\n    \"seedUrls\"\n  ],\n  \"example\": {\n    \"name\": \"my-seeds\",\n    \"seedUrls\": [\n      {\n        \"url\": \"https://example.com\"\n      },\n      {\n        \"url\": \"https://nutch.apache.org\"\n      }\n    ]\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-seed-list-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: SeedList
---
