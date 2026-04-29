---
description: A list of alert events for an SAP HANA Cloud service instance.
layout: schema
name: AlertEventList
properties_list:
- description: The list of alert events.
  name: items
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-alert-event-list-schema.json
slug: sap-hana-cloud-rest-alert-event-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlertEventList\",\n  \"type\": \"object\",\n  \"description\": \"A list of alert events for an SAP HANA Cloud service instance.\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of alert events.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-alert-event-list-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: AlertEventList
---
