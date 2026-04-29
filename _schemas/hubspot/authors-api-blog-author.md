---
description: Represents a blog author profile with biographical and social information
layout: schema
name: BlogAuthor
properties_list:
- description: Unique identifier for the blog author
  name: id
  type: string
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
- description: Language code for the author profile (e.g., en, es, fr)
  name: language
  type: string
- description: ID of the original author this was translated from
  name: translatedFromId
  type: string
- description: ISO 8601 timestamp when the author was created
  name: created
  type: string
- description: ISO 8601 timestamp when the author was last updated
  name: updated
  type: string
- description: ISO 8601 timestamp when the author was archived
  name: deletedAt
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/authors-api-blog-author-schema.json
slug: authors-api-blog-author
source_filename: authors-api-blog-author-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-blog-author-schema.json\",\n  \"title\": \"BlogAuthor\",\n  \"description\": \"Represents a blog author profile with biographical and social information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the blog author\",\n      \"example\": \"500123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the author\",\n      \"example\": \"Example Record\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly identifier for the author\",\n      \"example\": \"example-value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Author's email address\",\n      \"example\"\
  : \"jsmith@example.com\"\n    },\n    \"bio\": {\n      \"type\": \"string\",\n      \"description\": \"Author biography or description\",\n      \"example\": \"example-value\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Author's personal website URL\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    },\n    \"twitter\": {\n      \"type\": \"string\",\n      \"description\": \"Author's Twitter/X handle\",\n      \"example\": \"example-value\"\n    },\n    \"facebook\": {\n      \"type\": \"string\",\n      \"description\": \"Author's Facebook profile URL\",\n      \"example\": \"example-value\"\n    },\n    \"linkedin\": {\n      \"type\": \"string\",\n      \"description\": \"Author's LinkedIn profile URL\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    },\n    \"avatar\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the author's avatar\
  \ image\",\n      \"example\": \"https://app.hubspot.com/contacts/12345\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Language code for the author profile (e.g., en, es, fr)\",\n      \"example\": \"en\"\n    },\n    \"translatedFromId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the original author this was translated from\",\n      \"example\": \"500123\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the author was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the author was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"deletedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the author\
  \ was archived\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"created\",\n    \"updated\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/authors-api-blog-author-schema.json
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
title: BlogAuthor
---
