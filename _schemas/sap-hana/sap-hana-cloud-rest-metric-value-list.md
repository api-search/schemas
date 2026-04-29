---
description: A collection of metric data points for an SAP HANA Cloud service instance.
layout: schema
name: MetricValueList
properties_list:
- description: The list of metric series.
  name: metrics
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-metric-value-list-schema.json
slug: sap-hana-cloud-rest-metric-value-list
source_filename: sap-hana-cloud-rest-metric-value-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricValueList\",\n  \"type\": \"object\",\n  \"description\": \"A collection of metric data points for an SAP HANA Cloud service instance.\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"The list of metric series.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-metric-value-list-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: MetricValueList
---
