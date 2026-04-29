---
description: A collection of metering data points for billing and capacity tracking.
layout: schema
name: MeteringValueList
properties_list:
- description: The list of metering records.
  name: values
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-metering-value-list-schema.json
slug: sap-hana-cloud-rest-metering-value-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeteringValueList\",\n  \"type\": \"object\",\n  \"description\": \"A collection of metering data points for billing and capacity tracking.\",\n  \"properties\": {\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The list of metering records.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-metering-value-list-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: MeteringValueList
---
