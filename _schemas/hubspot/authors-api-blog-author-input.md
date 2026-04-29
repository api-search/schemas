---
description: Input data for creating or updating a blog author
layout: schema
name: BlogAuthorInput
properties_list:
- description: Full display name of the author
  name: name
  type: string
- description: URL-friendly identifier for the author
  name: slug
  type: string
- description: Author's email address
  name: email
  type: string
- description: Author biography or description
  name: bio
  type: string
- description: Author's personal website URL
  name: website
  type: string
- description: Author's Twitter/X handle
  name: twitter
  type: string
- description: Author's Facebook profile URL
  name: facebook
  type: string
- description: Author's LinkedIn profile URL
  name: linkedin
  type: string
- description: URL to the author's avatar image
  name: avatar
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-blog-author-input-schema.json
slug: authors-api-blog-author-input
source_filename: authors-api-blog-author-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-blog-author-input-schema.json\",\n  \"title\": \"BlogAuthorInput\",\n  \"description\": \"Input data for creating or updating a blog author\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the author\",\n      \"example\": \"Example Record\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly identifier for the author\",\n      \"example\": \"example-value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Author's email address\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"bio\": {\n      \"type\": \"string\",\n      \"description\": \"Author biography or description\",\n      \"example\":\
  \ \"example-value\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Author's personal website URL\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    },\n    \"twitter\": {\n      \"type\": \"string\",\n      \"description\": \"Author's Twitter/X handle\",\n      \"example\": \"example-value\"\n    },\n    \"facebook\": {\n      \"type\": \"string\",\n      \"description\": \"Author's Facebook profile URL\",\n      \"example\": \"example-value\"\n    },\n    \"linkedin\": {\n      \"type\": \"string\",\n      \"description\": \"Author's LinkedIn profile URL\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    },\n    \"avatar\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the author's avatar image\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-blog-author-input-schema.json
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
title: BlogAuthorInput
---
