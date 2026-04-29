---
description: ''
layout: schema
name: SearchJobList
properties_list:
- description: URI of the request
  name: origin
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: generator
  type: object
- description: ''
  name: entry
  type: array
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-enterprise-rest-search-job-list-schema.json
slug: splunk-enterprise-rest-search-job-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SearchJobList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"origin\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the request\"\n    },\n    \"updated\": {\n      \"type\": \"string\"\n    },\n    \"generator\": {\n      \"type\": \"object\"\n    },\n    \"entry\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-enterprise-rest-search-job-list-schema.json
tags:
- Analytics
- Data Analysis
- Logging
- Machine Data
- Monitoring
- Observability
- Platform
- Security
- SIEM
title: SearchJobList
---
