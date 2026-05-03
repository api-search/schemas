---
description: Standard paginated collection response pattern for RESTful web services. Supports both offset-based and cursor-based pagination.
layout: schema
name: REST Pagination Response
properties_list:
- description: Array of resource items for this page
  name: data
  type: array
- description: Pagination metadata
  name: meta
  type: object
- description: Navigation links for pagination
  name: links
  type: object
provider_name: RESTful Web Services
provider_slug: restful-web-services
schema_file: json-schema/restful-web-services-pagination-schema.json
slug: restful-web-services-pagination
source_filename: restful-web-services-pagination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/restful-web-services/schemas/pagination\",\n  \"title\": \"REST Pagination Response\",\n  \"description\": \"Standard paginated collection response pattern for RESTful web services. Supports both offset-based and cursor-based pagination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of resource items for this page\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination metadata\",\n      \"properties\": {\n        \"total\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of items across all pages\"\n        },\n        \"page\": {\n          \"type\": \"integer\",\n          \"description\": \"Current page number (1-based)\"\n        },\n        \"perPage\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Number of items per page\"\n        },\n        \"totalPages\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of pages\"\n        },\n        \"offset\": {\n          \"type\": \"integer\",\n          \"description\": \"Current offset (for offset-based pagination)\"\n        },\n        \"limit\": {\n          \"type\": \"integer\",\n          \"description\": \"Current limit (for offset-based pagination)\"\n        },\n        \"cursor\": {\n          \"type\": \"string\",\n          \"description\": \"Cursor for the next page (for cursor-based pagination)\"\n        },\n        \"hasMore\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether more pages are available\"\n        }\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Navigation links for pagination\",\n      \"properties\": {\n        \"self\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"first\": { \"type\": \"\
  string\", \"format\": \"uri\" },\n        \"prev\": { \"type\": [\"string\", \"null\"], \"format\": \"uri\" },\n        \"next\": { \"type\": [\"string\", \"null\"], \"format\": \"uri\" },\n        \"last\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    }\n  },\n  \"required\": [\"data\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/restful-web-services/refs/heads/main/json-schema/restful-web-services-pagination-schema.json
tags:
- Architecture
- HTTP
- REST
- Web Services
title: REST Pagination Response
---
