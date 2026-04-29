---
description: SharePoint search results.
layout: schema
name: SearchResult
properties_list:
- description: ''
  name: PrimaryQueryResult
  type: object
provider_name: Microsoft SharePoint
provider_slug: sharepoint
schema_file: json-schema/sharepoint-search-result-schema.json
slug: sharepoint-search-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-search-result-schema.json\",\n  \"title\": \"SearchResult\",\n  \"description\": \"SharePoint search results.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PrimaryQueryResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"RelevantResults\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"TotalRows\": {\n              \"type\": \"integer\",\n              \"example\": 42\n            },\n            \"RowCount\": {\n              \"type\": \"integer\",\n              \"example\": 10\n            },\n            \"Table\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Rows\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\",\n\
  \                    \"properties\": {\n                      \"Cells\": {\n                        \"type\": \"array\",\n                        \"items\": {\n                          \"type\": \"object\",\n                          \"properties\": {\n                            \"Key\": {\n                              \"type\": \"string\",\n                              \"example\": \"Title\"\n                            },\n                            \"Value\": {\n                              \"type\": \"string\",\n                              \"example\": \"Sample Document\"\n                            }\n                          }\n                        }\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sharepoint/refs/heads/main/json-schema/sharepoint-search-result-schema.json
tags:
- Collaboration
- Document Management
- Enterprise Content Management
- Intranet
- Microsoft
title: SearchResult
---
