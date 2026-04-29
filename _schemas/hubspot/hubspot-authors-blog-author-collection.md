---
description: Paginated collection of blog authors
layout: schema
name: BlogAuthorCollection
properties_list:
- description: Total number of authors matching the query
  name: total
  type: integer
- description: Array of blog authors
  name: results
  type: array
- description: Pagination information for navigating result sets
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-authors-blog-author-collection-schema.json
slug: hubspot-authors-blog-author-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Paginated collection of blog authors\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of authors matching the query\",\n      \"example\": 10\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of blog authors\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"name\": \"Example Record\",\n          \"slug\": \"example-value\",\n          \"email\": \"jsmith@example.com\",\n          \"bio\": \"example-value\",\n          \"website\": \"https://app.hubspot.com/contacts/12345\",\n          \"twitter\": \"example-value\",\n          \"facebook\": \"example-value\",\n          \"linkedin\": \"https://app.hubspot.com/contacts/12345\",\n          \"avatar\": \"https://app.hubspot.com/contacts/12345\",\n          \"language\": \"en\",\n          \"translatedFromId\": \"500123\",\n          \"created\": \"2025-03-15T14:30:00Z\"\
  ,\n          \"updated\": \"2025-03-15T14:30:00Z\",\n          \"deletedAt\": \"2025-03-15T14:30:00Z\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents a blog author profile with biographical and social information\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the blog author\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Full display name of the author\",\n            \"example\": \"Example Record\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"URL-friendly identifier for the author\",\n            \"example\": \"example-value\"\n          },\n          \"email\": {\n            \"type\": \"string\",\n            \"description\": \"Author's email address\",\n            \"format\"\
  : \"email\",\n            \"example\": \"jsmith@example.com\"\n          },\n          \"bio\": {\n            \"type\": \"string\",\n            \"description\": \"Author biography or description\",\n            \"example\": \"example-value\"\n          },\n          \"website\": {\n            \"type\": \"string\",\n            \"description\": \"Author's personal website URL\",\n            \"format\": \"uri\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"twitter\": {\n            \"type\": \"string\",\n            \"description\": \"Author's Twitter/X handle\",\n            \"example\": \"example-value\"\n          },\n          \"facebook\": {\n            \"type\": \"string\",\n            \"description\": \"Author's Facebook profile URL\",\n            \"example\": \"example-value\"\n          },\n          \"linkedin\": {\n            \"type\": \"string\",\n            \"description\": \"Author's LinkedIn profile URL\",\n     \
  \       \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"avatar\": {\n            \"type\": \"string\",\n            \"description\": \"URL to the author's avatar image\",\n            \"format\": \"uri\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"language\": {\n            \"type\": \"string\",\n            \"description\": \"Language code for the author profile (e.g., en, es, fr)\",\n            \"example\": \"en\"\n          },\n          \"translatedFromId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the original author this was translated from\",\n            \"example\": \"500123\"\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 timestamp when the author was created\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"updated\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 timestamp when the author was last updated\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"deletedAt\": {\n            \"type\": \"string\",\n            \"description\": \"ISO 8601 timestamp when the author was archived\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"name\",\n          \"created\",\n          \"updated\"\n        ]\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information for navigating result sets\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor for retrieving the next page of results\",\n          \"properties\": {\n            \"after\": {\n             \
  \ \"type\": \"string\",\n              \"description\": \"Cursor token for the next page\",\n              \"example\": \"example-value\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"API link to the next page of results\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"total\",\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlogAuthorCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-authors-blog-author-collection-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: BlogAuthorCollection
---
