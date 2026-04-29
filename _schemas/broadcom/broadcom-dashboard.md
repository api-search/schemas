---
description: A Dashboard represents a configurable visualization in Operations for Applications that displays metric data through charts, tables, and other widgets for monitoring and analysis.
layout: schema
name: Broadcom Dashboard
properties_list:
- description: The unique identifier of the dashboard.
  name: id
  type: string
- description: The display name of the dashboard.
  name: name
  type: string
- description: A description of the dashboard.
  name: description
  type: string
- description: The URL slug used to access the dashboard.
  name: url
  type: string
- description: Tags associated with the dashboard.
  name: tags
  type: object
- description: The sections of the dashboard containing rows of charts.
  name: sections
  type: array
- description: The identifier of the user who created the dashboard.
  name: creatorId
  type: string
- description: The identifier of the user who last updated the dashboard.
  name: updaterId
  type: string
- description: The creation timestamp in epoch milliseconds.
  name: createdEpochMillis
  type: integer
- description: The last update timestamp in epoch milliseconds.
  name: updatedEpochMillis
  type: integer
- description: Dashboard parameters for dynamic filtering.
  name: parameters
  type: object
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-dashboard-schema.json
slug: broadcom-dashboard
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/broadcom/blob/main/json-schema/broadcom-dashboard-schema.json\",\n  \"title\": \"Broadcom Dashboard\",\n  \"description\": \"A Dashboard represents a configurable visualization in Operations for Applications that displays metric data through charts, tables, and other widgets for monitoring and analysis.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the dashboard.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the dashboard.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the dashboard.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL slug used to access the dashboard.\"\n    },\n    \"tags\": {\n      \"type\": \"\
  object\",\n      \"properties\": {\n        \"customerTags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"User-defined tags for the dashboard.\"\n        }\n      },\n      \"description\": \"Tags associated with the dashboard.\"\n    },\n    \"sections\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the dashboard section.\"\n          },\n          \"rows\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"charts\": {\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"name\": {\n                        \"type\"\
  : \"string\",\n                        \"description\": \"The name of the chart.\"\n                      },\n                      \"sources\": {\n                        \"type\": \"array\",\n                        \"items\": {\n                          \"type\": \"object\",\n                          \"properties\": {\n                            \"name\": {\n                              \"type\": \"string\",\n                              \"description\": \"The name of the data source.\"\n                            },\n                            \"query\": {\n                              \"type\": \"string\",\n                              \"description\": \"The query expression for the data source.\"\n                            }\n                          }\n                        },\n                        \"description\": \"The data sources for the chart.\"\n                      },\n                      \"chartSettings\": {\n                        \"type\": \"object\"\
  ,\n                        \"description\": \"Display settings for the chart.\"\n                      }\n                    }\n                  },\n                  \"description\": \"The charts in this row.\"\n                }\n              }\n            },\n            \"description\": \"The rows in this section.\"\n          }\n        }\n      },\n      \"description\": \"The sections of the dashboard containing rows of charts.\"\n    },\n    \"creatorId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user who created the dashboard.\"\n    },\n    \"updaterId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the user who last updated the dashboard.\"\n    },\n    \"createdEpochMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"The creation timestamp in epoch milliseconds.\"\n    },\n    \"updatedEpochMillis\": {\n      \"type\": \"integer\",\n      \"description\": \"The last update timestamp in epoch\
  \ milliseconds.\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Dashboard parameters for dynamic filtering.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/json-schema/broadcom-dashboard-schema.json
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Dashboard
---
