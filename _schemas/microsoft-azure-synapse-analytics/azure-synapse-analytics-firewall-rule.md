---
description: An IP firewall rule that controls network access to a Synapse workspace.
layout: schema
name: Azure Synapse Analytics Firewall Rule
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-firewall-rule-schema.json
slug: azure-synapse-analytics-firewall-rule
source_filename: azure-synapse-analytics-firewall-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-firewall-rule-schema.json\",\n  \"title\": \"Azure Synapse Analytics Firewall Rule\",\n  \"description\": \"An IP firewall rule that controls network access to a Synapse workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"startIpAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The start IP address of the firewall rule (IPv4 format).\"\n        },\n        \"endIpAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The end IP address of the firewall rule (IPv4\
  \ format).\"\n        },\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\"Provisioning\", \"Succeeded\", \"Deleting\", \"Failed\", \"DeleteError\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-firewall-rule-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Firewall Rule
---
