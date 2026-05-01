---
description: A presidential transcript record from FiscalNote's PolicyNote API, delivering primary-source verified transcripts of presidential communications including executive orders, proclamations, press statements, and public remarks.
layout: schema
name: FiscalNote Presidential Transcript
properties_list:
- description: Unique identifier for the transcript record.
  name: id
  type: string
- description: Title of the transcript.
  name: title
  type: string
- description: Type of presidential communication.
  name: type
  type: string
- description: Date of the communication in ISO 8601 format.
  name: date
  type: string
- description: Location where the communication took place.
  name: location
  type: string
- description: Duration of the communication in ISO 8601 duration format.
  name: duration
  type: string
- description: Total word count of the transcript.
  name: wordCount
  type: integer
- description: Full text of the transcript.
  name: fullText
  type: string
- description: Summary of the transcript content.
  name: summary
  type: string
- description: URL to the video recording if available.
  name: videoUrl
  type: string
- description: URL to the primary source document.
  name: sourceUrl
  type: string
- description: Indicates whether this transcript has been verified against the primary source.
  name: verified
  type: boolean
- description: Timestamp when the record was created.
  name: createdAt
  type: string
- description: Timestamp when the record was last updated.
  name: updatedAt
  type: string
provider_name: FiscalNote
provider_slug: fiscalnote
schema_file: json-schema/fiscalnote-transcript-schema.json
slug: fiscalnote-transcript
source_filename: fiscalnote-transcript-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fiscalnote.com/schemas/fiscalnote/transcript.json\",\n  \"title\": \"FiscalNote Presidential Transcript\",\n  \"description\": \"A presidential transcript record from FiscalNote's PolicyNote API, delivering primary-source verified transcripts of presidential communications including executive orders, proclamations, press statements, and public remarks.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"title\", \"type\", \"date\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the transcript record.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the transcript.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of presidential communication.\",\n      \"enum\": [\"executive_order\", \"proclamation\", \"press_statement\", \"public_remarks\"\
  , \"interview\", \"formal_event\"]\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of the communication in ISO 8601 format.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Location where the communication took place.\"\n    },\n    \"duration\": {\n      \"type\": \"string\",\n      \"description\": \"Duration of the communication in ISO 8601 duration format.\",\n      \"pattern\": \"^P(?:\\\\d+D)?(?:T(?:\\\\d+H)?(?:\\\\d+M)?(?:\\\\d+S)?)?$\"\n    },\n    \"wordCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total word count of the transcript.\",\n      \"minimum\": 0\n    },\n    \"fullText\": {\n      \"type\": \"string\",\n      \"description\": \"Full text of the transcript.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Summary of the transcript content.\"\n    },\n    \"videoUrl\": {\n      \"type\": \"string\",\n      \"\
  format\": \"uri\",\n      \"description\": \"URL to the video recording if available.\"\n    },\n    \"sourceUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the primary source document.\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this transcript has been verified against the primary source.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/json-schema/fiscalnote-transcript-schema.json
tags:
- Government
- Legislation
- Policy
- Political Intelligence
- Regulation
title: FiscalNote Presidential Transcript
---
