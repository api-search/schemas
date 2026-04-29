---
description: Request body for creating a CMS page.
layout: schema
name: PageCreateRequest
properties_list:
- description: The internal name of the page.
  name: name
  type: string
- description: The HTML title tag content.
  name: htmlTitle
  type: string
- description: The URL slug for the page.
  name: slug
  type: string
- description: The meta description for SEO.
  name: metaDescription
  type: string
- description: The domain to host the page on.
  name: domain
  type: string
- description: The language code for the page content.
  name: language
  type: string
- description: The path to the template to use for the page.
  name: templatePath
  type: string
- description: The layout sections and widget data for the page content.
  name: layoutSections
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/cms-pages-api-page-create-request-schema.json
slug: cms-pages-api-page-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-pages-api-page-create-request-schema.json\",\n  \"title\": \"PageCreateRequest\",\n  \"description\": \"Request body for creating a CMS page.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The internal name of the page.\",\n      \"example\": \"Example Record\"\n    },\n    \"htmlTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The HTML title tag content.\",\n      \"example\": \"Example Record\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL slug for the page.\",\n      \"example\": \"example-value\"\n    },\n    \"metaDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The meta description for SEO.\",\n      \"example\": \"This is an example description.\"\
  \n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain to host the page on.\",\n      \"example\": \"example.hubspot.com\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The language code for the page content.\",\n      \"example\": \"en\"\n    },\n    \"templatePath\": {\n      \"type\": \"string\",\n      \"description\": \"The path to the template to use for the page.\",\n      \"example\": \"/content/templates/example\"\n    },\n    \"layoutSections\": {\n      \"type\": \"object\",\n      \"description\": \"The layout sections and widget data for the page content.\",\n      \"additionalProperties\": true,\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"slug\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/cms-pages-api-page-create-request-schema.json
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
title: PageCreateRequest
---
