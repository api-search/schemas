---
description: Request body for creating a new instance mapping.
layout: schema
name: CreateInstanceMappingRequest
properties_list:
- description: The target subaccount identifier for the mapping.
  name: targetSubaccountId
  type: string
- description: The target environment instance identifier.
  name: targetEnvironmentInstanceId
  type: string
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-create-instance-mapping-request-schema.json
slug: sap-hana-cloud-rest-create-instance-mapping-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateInstanceMappingRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new instance mapping.\",\n  \"properties\": {\n    \"targetSubaccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The target subaccount identifier for the mapping.\"\n    },\n    \"targetEnvironmentInstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The target environment instance identifier.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-create-instance-mapping-request-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: CreateInstanceMappingRequest
---
