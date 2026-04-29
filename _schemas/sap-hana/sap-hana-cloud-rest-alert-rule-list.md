---
description: A list of alert rules configured for an SAP HANA Cloud service instance.
layout: schema
name: AlertRuleList
properties_list:
- description: The list of alert rules.
  name: items
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-alert-rule-list-schema.json
slug: sap-hana-cloud-rest-alert-rule-list
source_filename: sap-hana-cloud-rest-alert-rule-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlertRuleList\",\n  \"type\": \"object\",\n  \"description\": \"A list of alert rules configured for an SAP HANA Cloud service instance.\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of alert rules.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-alert-rule-list-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: AlertRuleList
---
