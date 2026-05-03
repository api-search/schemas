---
description: A search response from the Reuters Connect API containing a list of content items matching the search criteria, along with metadata about the total result count and the query that was executed.
layout: schema
name: Reuters Connect Search Result
properties_list:
- description: Array of content item summaries matching the search criteria.
  name: results
  type: array
- description: Total number of items matching the search criteria across all pages.
  name: totalResults
  type: integer
- description: The search query string that was executed.
  name: query
  type: string
provider_name: Reuters
provider_slug: reuters
schema_file: json-schema/reuters-search-result-schema.json
slug: reuters-search-result
source_filename: reuters-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/reuters/json-schema/reuters-search-result-schema.json\",\n  \"title\": \"Reuters Connect Search Result\",\n  \"description\": \"A search response from the Reuters Connect API containing a list of content items matching the search criteria, along with metadata about the total result count and the query that was executed.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"results\",\n    \"totalResults\"\n  ],\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of content item summaries matching the search criteria.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/itemSummary\"\n      }\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of items matching the search criteria across all pages.\",\n      \"minimum\": 0\n    },\n    \"query\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The search query string that was executed.\"\n    }\n  },\n  \"$defs\": {\n    \"itemSummary\": {\n      \"type\": \"object\",\n      \"description\": \"A summary representation of a content item containing key metadata for display in search results without the full content body.\",\n      \"required\": [\n        \"id\",\n        \"headline\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the item, typically in tag URI format.\",\n          \"examples\": [\n            \"tag:reuters.com,2025:newsml_L1N3KT0AB:1\"\n          ]\n        },\n        \"guid\": {\n          \"type\": \"string\",\n          \"description\": \"A globally unique identifier for the item regardless of version.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The version number of this item revision.\"\n        },\n        \"headline\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The headline or title of the content item.\"\n        },\n        \"dateCreated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the item was originally created.\"\n        },\n        \"dateModified\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time when the item was last modified.\"\n        },\n        \"channel\": {\n          \"type\": \"string\",\n          \"description\": \"The alias of the channel this item belongs to.\"\n        },\n        \"mediaType\": {\n          \"type\": \"string\",\n          \"description\": \"The media type of the content.\",\n          \"enum\": [\n            \"TEXT\",\n            \"PICTURE\",\n            \"VIDEO\",\n            \"GRAPHIC\",\n            \"COMPOSITE\"\n          ]\n        },\n        \"slug\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"A short keyword slug summarizing the item topic.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/json-schema/reuters-search-result-schema.json
tags:
- Business
- Finance
- Journalism
- Media
- News
- Wire Service
title: Reuters Connect Search Result
---
