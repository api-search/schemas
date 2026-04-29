---
description: Defines a group of related metrics collected for a target. Each metric group has a name, collection frequency, and a set of metric columns.
layout: schema
name: MetricGroup
properties_list:
- description: Unique name of the metric group.
  name: metricGroupName
  type: string
- description: Human-readable display name.
  name: displayName
  type: string
- description: Description of what this metric group measures.
  name: description
  type: string
- description: Collection interval in seconds.
  name: collectionFrequency
  type: integer
- description: List of metric columns in this group.
  name: metricColumns
  type: array
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-metric-group-schema.json
slug: oracle-enterprise-manager-cloud-control-metric-group
source_filename: oracle-enterprise-manager-cloud-control-metric-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricGroup\",\n  \"type\": \"object\",\n  \"description\": \"Defines a group of related metrics collected for a target. Each metric group has a name, collection frequency, and a set of metric columns.\",\n  \"properties\": {\n    \"metricGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the metric group.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what this metric group measures.\"\n    },\n    \"collectionFrequency\": {\n      \"type\": \"integer\",\n      \"description\": \"Collection interval in seconds.\"\n    },\n    \"metricColumns\": {\n      \"type\": \"array\",\n      \"description\": \"List of metric columns in this group.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-metric-group-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: MetricGroup
---
