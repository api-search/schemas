---
description: Acuity Brands product or content web page
layout: schema
name: Webpage
properties_list:
- description: Page identifier
  name: pageId
  type: string
- description: Canonical page URL
  name: url
  type: string
- description: Page title
  name: title
  type: string
- description: Page type
  name: type
  type: string
- description: Associated brand
  name: brand
  type: string
- description: SEO meta description
  name: metaDescription
  type: string
- description: Associated product number if product page
  name: productNumber
  type: string
- description: Page last modified timestamp
  name: lastModified
  type: string
provider_name: acuity-brands
provider_slug: acuity-brands
schema_file: json-schema/acuity-brands-webpage-schema.json
slug: acuity-brands-webpage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12\",\n  \"$id\": \"https://schema.api-evangelist.com/acuity-brands/acuity-brands-webpage-schema.json\",\n  \"title\": \"Webpage\",\n  \"description\": \"Acuity Brands product or content web page\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pageId\": {\n      \"type\": \"string\",\n      \"description\": \"Page identifier\",\n      \"example\": \"lithonia-lbl4\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Canonical page URL\",\n      \"example\": \"https://www.acuitybrands.com/products/lbl4\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Page title\",\n      \"example\": \"LBL4 LED Wrap Light\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"product\",\n        \"category\",\n        \"landing\",\n        \"support\"\n      ],\n      \"description\": \"Page type\",\n      \"example\": \"product\"\n    },\n\
  \    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Associated brand\",\n      \"example\": \"Lithonia Lighting\"\n    },\n    \"metaDescription\": {\n      \"type\": \"string\",\n      \"description\": \"SEO meta description\"\n    },\n    \"productNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Associated product number if product page\",\n      \"example\": \"LBL4 48L ADP\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Page last modified timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acuity-brands/refs/heads/main/json-schema/acuity-brands-webpage-schema.json
tags: []
title: Webpage
---
