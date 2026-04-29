---
description: A list of instance mappings for an SAP HANA Cloud service instance.
layout: schema
name: InstanceMappingList
properties_list:
- description: The list of instance mappings.
  name: items
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-instance-mapping-list-schema.json
slug: sap-hana-cloud-rest-instance-mapping-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceMappingList\",\n  \"type\": \"object\",\n  \"description\": \"A list of instance mappings for an SAP HANA Cloud service instance.\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"The list of instance mappings.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-instance-mapping-list-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: InstanceMappingList
---
