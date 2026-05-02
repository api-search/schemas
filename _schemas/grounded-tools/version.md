---
description: A specific indexed version of a library's documentation, including metadata about the indexing process and document counts.
layout: schema
name: grounded.tools Version
properties_list:
- description: Version string. Supports full semver (1.2.3), pre-release (1.2.3-beta.1), or partial (1, 1.2).
  name: version
  type: string
- description: Number of indexed documents for this version.
  name: documentCount
  type: integer
- description: Number of unique URLs indexed for this version.
  name: uniqueUrlCount
  type: integer
- description: Timestamp when the version was indexed.
  name: indexedAt
  type: string
- description: Current status of the version in the store.
  name: status
  type: string
- description: Original source URL used for scraping this version's documentation.
  name: sourceUrl
  type: string
provider_name: Grounded.tools
provider_slug: grounded-tools
schema_file: json-schema/version.json
slug: version
source_filename: version.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/grounded-tools/blob/main/json-schema/version.json\",\n  \"title\": \"grounded.tools Version\",\n  \"description\": \"A specific indexed version of a library's documentation, including metadata about the indexing process and document counts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Version string. Supports full semver (1.2.3), pre-release (1.2.3-beta.1), or partial (1, 1.2).\"\n    },\n    \"documentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of indexed documents for this version.\"\n    },\n    \"uniqueUrlCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unique URLs indexed for this version.\"\n    },\n    \"indexedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"description\"\
  : \"Timestamp when the version was indexed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the version in the store.\"\n    },\n    \"sourceUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"description\": \"Original source URL used for scraping this version's documentation.\"\n    }\n  },\n  \"required\": [\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/grounded-tools/refs/heads/main/json-schema/version.json
tags:
- Developer Tools
- Developers
- Documentation
- Experience
title: grounded.tools Version
---
