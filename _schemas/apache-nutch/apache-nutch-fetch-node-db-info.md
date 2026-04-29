---
description: Information about a fetched node in the FetchDB.
layout: schema
name: FetchNodeDbInfo
properties_list:
- description: The URL of the fetched node.
  name: url
  type: string
- description: The HTTP status code of the fetch.
  name: status
  type: integer
- description: The number of outgoing links discovered.
  name: numOfOutlinks
  type: integer
- description: The outgoing links from this node.
  name: children
  type: array
provider_name: Apache Nutch
provider_slug: apache-nutch
schema_file: json-schema/apache-nutch-fetch-node-db-info-schema.json
slug: apache-nutch-fetch-node-db-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-fetch-node-db-info-schema.json\",\n  \"title\": \"FetchNodeDbInfo\",\n  \"description\": \"Information about a fetched node in the FetchDB.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the fetched node.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"minimum\": 0,\n      \"maximum\": 2147483647,\n      \"description\": \"The HTTP status code of the fetch.\"\n    },\n    \"numOfOutlinks\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"minimum\": 0,\n      \"maximum\": 2147483647,\n      \"description\": \"The number of outgoing links discovered.\"\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"\
  type\": \"object\",\n        \"description\": \"A child (outlink) of a fetched node.\",\n        \"properties\": {\n          \"childUrl\": {\n            \"type\": \"string\",\n            \"description\": \"The URL of the child node.\"\n          },\n          \"anchorText\": {\n            \"type\": \"string\",\n            \"description\": \"The anchor text of the link.\"\n          }\n        }\n      },\n      \"description\": \"The outgoing links from this node.\"\n    }\n  },\n  \"required\": [\n    \"children\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/json-schema/apache-nutch-fetch-node-db-info-schema.json
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
title: FetchNodeDbInfo
---
