---
description: A saved search (KQL query) in a Log Analytics workspace.
layout: schema
name: SavedSearch
properties_list:
- description: Fully qualified resource ID.
  name: id
  type: string
- description: The name of the resource.
  name: name
  type: string
- description: The type of the resource.
  name: type
  type: string
- description: The ETag of the saved search.
  name: etag
  type: string
- description: Saved search properties.
  name: properties
  type: object
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
schema_file: json-schema/management-api-saved-search-schema.json
slug: management-api-saved-search
source_filename: management-api-saved-search-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/management-api-saved-search-schema.json\",\n  \"title\": \"SavedSearch\",\n  \"description\": \"A saved search (KQL query) in a Log Analytics workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified resource ID.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource.\",\n      \"readOnly\": true\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the resource.\",\n      \"readOnly\": true\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the saved search.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Saved search\
  \ properties.\",\n      \"required\": [\"category\", \"displayName\", \"query\"],\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"The category of the saved search.\",\n          \"example\": \"General Exploration\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Saved search display name.\",\n          \"example\": \"All Events\"\n        },\n        \"query\": {\n          \"type\": \"string\",\n          \"description\": \"The KQL query expression.\",\n          \"example\": \"Event | sort by TimeGenerated desc\"\n        },\n        \"functionAlias\": {\n          \"type\": \"string\",\n          \"description\": \"The function alias if query serves as a function.\"\n        },\n        \"functionParameters\": {\n          \"type\": \"string\",\n          \"description\": \"The optional function parameters.\"\n        },\n        \"version\": {\n          \"type\"\
  : \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The version number of the query language.\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"description\": \"The tags attached to the saved search.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/management-api-saved-search-schema.json
tags:
- Analytics
- Azure
- Cloud
- Logging
- Monitoring
title: SavedSearch
---
