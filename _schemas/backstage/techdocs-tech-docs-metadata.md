---
description: TechDocsMetadata schema from Backstage techdocs API
layout: schema
name: TechDocsMetadata
properties_list:
- description: The name of the documentation site.
  name: site_name
  type: string
- description: Description of the documentation site.
  name: site_description
  type: string
- description: ETag for cache validation.
  name: etag
  type: string
- description: Timestamp of the last documentation build.
  name: build_timestamp
  type: string
- description: List of files in the documentation bundle.
  name: files
  type: array
provider_name: Backstage
provider_slug: backstage
schema_file: json-schema/techdocs-tech-docs-metadata-schema.json
slug: techdocs-tech-docs-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/techdocs-tech-docs-metadata-schema.json\",\n  \"title\": \"TechDocsMetadata\",\n  \"description\": \"TechDocsMetadata schema from Backstage techdocs API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"site_name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the documentation site.\"\n    },\n    \"site_description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the documentation site.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for cache validation.\"\n    },\n    \"build_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last documentation build.\"\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\"\
  : \"string\"\n      },\n      \"description\": \"List of files in the documentation bundle.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backstage/refs/heads/main/json-schema/techdocs-tech-docs-metadata-schema.json
tags:
- Developer Portal
- Internal Developer Platform
- Software Catalog
- Open Source
title: TechDocsMetadata
---
