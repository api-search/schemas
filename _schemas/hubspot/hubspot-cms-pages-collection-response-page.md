---
description: A paginated list of CMS pages.
layout: schema
name: CollectionResponsePage
properties_list:
- description: ''
  name: results
  type: array
- description: Pagination information.
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-cms-pages-collection-response-page-schema.json
slug: hubspot-cms-pages-collection-response-page
source_filename: hubspot-cms-pages-collection-response-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated list of CMS pages.\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"name\": \"Example Record\",\n          \"htmlTitle\": \"Example Record\",\n          \"slug\": \"example-value\",\n          \"state\": \"DRAFT\",\n          \"currentState\": \"active\",\n          \"contentTypeCategory\": 100,\n          \"publishDate\": \"2025-03-15T14:30:00Z\",\n          \"metaDescription\": \"This is an example description.\",\n          \"url\": \"https://app.hubspot.com/contacts/12345\",\n          \"domain\": \"example.hubspot.com\",\n          \"language\": \"en\",\n          \"templatePath\": \"/content/templates/example\",\n          \"createdAt\": \"2025-03-15T14:30:00Z\",\n          \"updatedAt\": \"2025-03-15T14:30:00Z\",\n          \"archived\": true\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\"\
  ,\n        \"description\": \"A HubSpot CMS page (site page or landing page).\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the page.\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The internal name of the page.\",\n            \"example\": \"Example Record\"\n          },\n          \"htmlTitle\": {\n            \"type\": \"string\",\n            \"description\": \"The HTML title tag content for the page.\",\n            \"example\": \"Example Record\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The URL slug for the page.\",\n            \"example\": \"example-value\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"description\": \"The current publish state of the page.\",\n            \"example\"\
  : \"DRAFT\",\n            \"enum\": [\n              \"DRAFT\",\n              \"PUBLISHED\",\n              \"ARCHIVED\"\n            ]\n          },\n          \"currentState\": {\n            \"type\": \"string\",\n            \"description\": \"The current display state of the page.\",\n            \"example\": \"active\"\n          },\n          \"contentTypeCategory\": {\n            \"type\": \"integer\",\n            \"description\": \"The content type category code.\",\n            \"example\": 100\n          },\n          \"publishDate\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the page was or will be published.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"metaDescription\": {\n            \"type\": \"string\",\n            \"description\": \"The meta description for SEO.\",\n            \"example\": \"This is an example description.\"\n          },\n   \
  \       \"url\": {\n            \"type\": \"string\",\n            \"description\": \"The full URL of the published page.\",\n            \"example\": \"https://app.hubspot.com/contacts/12345\"\n          },\n          \"domain\": {\n            \"type\": \"string\",\n            \"description\": \"The domain the page is hosted on.\",\n            \"example\": \"example.hubspot.com\"\n          },\n          \"language\": {\n            \"type\": \"string\",\n            \"description\": \"The language code for the page content.\",\n            \"example\": \"en\"\n          },\n          \"templatePath\": {\n            \"type\": \"string\",\n            \"description\": \"The path to the template used by the page.\",\n            \"example\": \"/content/templates/example\"\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the page was created.\",\n            \"format\": \"date-time\",\n            \"example\"\
  : \"2025-03-15T14:30:00Z\"\n          },\n          \"updatedAt\": {\n            \"type\": \"string\",\n            \"description\": \"The date and time the page was last updated.\",\n            \"format\": \"date-time\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the page has been archived.\",\n            \"example\": true\n          }\n        }\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information.\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"after\": \"example-value\"\n          },\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectionResponsePage\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-cms-pages-collection-response-page-schema.json
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
title: CollectionResponsePage
---
