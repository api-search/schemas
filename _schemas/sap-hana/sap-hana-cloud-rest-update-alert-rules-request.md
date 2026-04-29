---
description: Request body for updating alert rules.
layout: schema
name: UpdateAlertRulesRequest
properties_list:
- description: The list of alert rule updates to apply.
  name: rules
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-update-alert-rules-request-schema.json
slug: sap-hana-cloud-rest-update-alert-rules-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateAlertRulesRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating alert rules.\",\n  \"properties\": {\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"The list of alert rule updates to apply.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-update-alert-rules-request-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: UpdateAlertRulesRequest
---
