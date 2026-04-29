---
description: VerifiedQuery represents a (question, sql) pair that has been manually verified (e.g. by an analyst) to be correct.
layout: schema
name: VerifiedQuery
properties_list:
- description: A name for this verified query. Mainly used for display purposes.
  name: name
  type: string
- description: The question being answered.
  name: question
  type: string
- description: The correct SQL query for answering the question.
  name: sql
  type: string
- description: Timestamp at which the query was last verified - measures in seconds since epoch, in UTC.
  name: verified_at
  type: integer
- description: Name of the person who verified this query.
  name: verified_by
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/cortex-analyst-verified-query-schema.json
slug: cortex-analyst-verified-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VerifiedQuery\",\n  \"type\": \"object\",\n  \"description\": \"VerifiedQuery represents a (question, sql) pair that has been manually verified (e.g. by an analyst) to be correct.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A name for this verified query. Mainly used for display purposes.\"\n    },\n    \"question\": {\n      \"type\": \"string\",\n      \"description\": \"The question being answered.\"\n    },\n    \"sql\": {\n      \"type\": \"string\",\n      \"description\": \"The correct SQL query for answering the question.\"\n    },\n    \"verified_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Timestamp at which the query was last verified - measures in seconds since epoch, in UTC.\"\n    },\n    \"verified_by\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the person who verified this query.\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/cortex-analyst-verified-query-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: VerifiedQuery
---
