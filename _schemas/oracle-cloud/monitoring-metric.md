---
description: A metric definition.
layout: schema
name: Metric
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: namespace
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: dimensions
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/monitoring-metric-schema.json
slug: monitoring-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-metric-schema.json\",\n  \"title\": \"Metric\",\n  \"description\": \"A metric definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"CpuUtilization\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"example\": \"oci_computeagent\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"dimensions\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-metric-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Metric
---
