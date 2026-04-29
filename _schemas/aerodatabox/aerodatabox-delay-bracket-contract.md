---
description: Delay bracket contract describing how many records are subject to a specific delay range
layout: schema
name: DelayBracketContract
properties_list:
- description: 'The beginning of the delay range (format: [-]hh:mm:ss). E.g. in the expresssion "delayed from 30 to 60 minutes" stands for "from 30 minutes". Value can be negative (therefore, means early occurence). '
  name: delayedFrom
  type: string
- description: 'The end of the delay range (format: [-]hh:mm:ss). E.g. in the expresssion "delayed from 30 to 60 minutes" stands for "to 60 minutes". Value can be negative (therefore, means early occurence). Must be '
  name: delayedTo
  type: string
- description: Count of records subject to a specified delay range
  name: num
  type: integer
- description: Percentage of records subject to a specified delay range. Only available when this delay bracket is provided as a part of a statistical information of a bigger context and the "total" count of records
  name: percentage
  type: number
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-delay-bracket-contract-schema.json
slug: aerodatabox-delay-bracket-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-delay-bracket-contract-schema.json\",\n  \"title\": \"DelayBracketContract\",\n  \"description\": \"Delay bracket contract describing how many records are subject to a specific delay range\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"delayedFrom\": {\n      \"type\": \"string\",\n      \"description\": \"The beginning of the delay range (format: [-]hh:mm:ss).\\r\\nE.g. in the expresssion \\\"delayed from 30 to 60 minutes\\\" stands for \\\"from 30 minutes\\\".\\r\\nValue can be negative (therefore, means early occurence).\\r\\n\\r\\nMust be preset if \\\"DelayedTo\\\" is not specified.\",\n      \"format\": \"date-span\",\n      \"nullable\": true\n    },\n    \"delayedTo\": {\n      \"type\": \"string\",\n      \"description\": \"The end of the delay range (format: [-]hh:mm:ss).\\r\\\
  nE.g. in the expresssion \\\"delayed from 30 to 60 minutes\\\" stands for \\\"to 60 minutes\\\".\\r\\nValue can be negative (therefore, means early occurence).\\r\\n\\r\\nMust be preset if \\\"DelayedFrom\\\" is not specified.\",\n      \"format\": \"date-span\",\n      \"nullable\": true\n    },\n    \"num\": {\n      \"type\": \"integer\",\n      \"description\": \"Count of records subject to a specified delay range\",\n      \"format\": \"int32\"\n    },\n    \"percentage\": {\n      \"type\": \"number\",\n      \"description\": \"Percentage of records subject to a specified delay range.\\r\\n\\r\\nOnly available when this delay bracket is provided as a part\\r\\nof a statistical information of a bigger context and the \\\"total\\\"\\r\\ncount of records is known.\",\n      \"format\": \"float\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"num\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-delay-bracket-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: DelayBracketContract
---
