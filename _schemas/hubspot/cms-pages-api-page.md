---
description: A HubSpot CMS page (site page or landing page).
layout: schema
name: Page
properties_list:
- description: The unique identifier for the page.
  name: id
  type: string
- description: The internal name of the page.
  name: name
  type: string
- description: The HTML title tag content for the page.
  name: htmlTitle
  type: string
- description: The URL slug for the page.
  name: slug
  type: string
- description: The current publish state of the page.
  name: state
  type: string
- description: The current display state of the page.
  name: currentState
  type: string
- description: The content type category code.
  name: contentTypeCategory
  type: integer
- description: The date and time the page was or will be published.
  name: publishDate
  type: string
- description: The meta description for SEO.
  name: metaDescription
  type: string
- description: The full URL of the published page.
  name: url
  type: string
- description: The domain the page is hosted on.
  name: domain
  type: string
- description: The language code for the page content.
  name: language
  type: string
- description: The path to the template used by the page.
  name: templatePath
  type: string
- description: The date and time the page was created.
  name: createdAt
  type: string
- description: The date and time the page was last updated.
  name: updatedAt
  type: string
- description: Whether the page has been archived.
  name: archived
  type: boolean
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/cms-pages-api-page-schema.json
slug: cms-pages-api-page
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-pages-api-page-schema.json\",\n  \"title\": \"Page\",\n  \"description\": \"A HubSpot CMS page (site page or landing page).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the page.\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The internal name of the page.\",\n      \"example\": \"Example Record\"\n    },\n    \"htmlTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The HTML title tag content for the page.\",\n      \"example\": \"Example Record\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL slug for the page.\",\n      \"example\": \"example-value\"\n    },\n    \"state\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The current publish state of the page.\",\n      \"enum\": [\n        \"DRAFT\",\n        \"PUBLISHED\",\n        \"ARCHIVED\"\n      ],\n      \"example\": \"DRAFT\"\n    },\n    \"currentState\": {\n      \"type\": \"string\",\n      \"description\": \"The current display state of the page.\",\n      \"example\": \"active\"\n    },\n    \"contentTypeCategory\": {\n      \"type\": \"integer\",\n      \"description\": \"The content type category code.\",\n      \"example\": 100\n    },\n    \"publishDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the page was or will be published.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"metaDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The meta description for SEO.\",\n      \"example\": \"This is an example description.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The full URL of the published page.\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain the page is hosted on.\",\n      \"example\": \"example.hubspot.com\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The language code for the page content.\",\n      \"example\": \"en\"\n    },\n    \"templatePath\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the template used by the page.\",\n      \"example\": \"/content/templates/example\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the page was created.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the page was last updated.\",\n      \"example\"\
  : \"2025-03-15T14:30:00Z\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the page has been archived.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-pages-api-page-schema.json
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
title: Page
---
