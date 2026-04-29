---
description: A single metric column within a metric group.
layout: schema
name: MetricColumn
properties_list:
- description: Name of the metric column.
  name: columnName
  type: string
- description: Human-readable display name.
  name: displayName
  type: string
- description: Data type of the metric column.
  name: columnType
  type: string
- description: Whether this column is a key column.
  name: isKey
  type: boolean
- description: Unit of measurement for the metric.
  name: unit
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-metric-column-schema.json
slug: oracle-enterprise-manager-cloud-control-metric-column
source_filename: oracle-enterprise-manager-cloud-control-metric-column-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricColumn\",\n  \"type\": \"object\",\n  \"description\": \"A single metric column within a metric group.\",\n  \"properties\": {\n    \"columnName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the metric column.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name.\"\n    },\n    \"columnType\": {\n      \"type\": \"string\",\n      \"description\": \"Data type of the metric column.\"\n    },\n    \"isKey\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this column is a key column.\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement for the metric.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-metric-column-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: MetricColumn
---
