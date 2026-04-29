---
description: An instance mapping that associates an SAP HANA Cloud service instance with a target in another subaccount or environment.
layout: schema
name: InstanceMapping
properties_list:
- description: The unique identifier of the instance mapping.
  name: mappingId
  type: string
- description: The source service instance identifier.
  name: serviceInstanceId
  type: string
- description: The target subaccount identifier.
  name: targetSubaccountId
  type: string
- description: The target environment instance identifier.
  name: targetEnvironmentInstanceId
  type: string
- description: ISO 8601 timestamp when the mapping was created.
  name: createdAt
  type: string
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-instance-mapping-schema.json
slug: sap-hana-cloud-rest-instance-mapping
source_filename: sap-hana-cloud-rest-instance-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceMapping\",\n  \"type\": \"object\",\n  \"description\": \"An instance mapping that associates an SAP HANA Cloud service instance with a target in another subaccount or environment.\",\n  \"properties\": {\n    \"mappingId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the instance mapping.\"\n    },\n    \"serviceInstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The source service instance identifier.\"\n    },\n    \"targetSubaccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The target subaccount identifier.\"\n    },\n    \"targetEnvironmentInstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The target environment instance identifier.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the mapping was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-instance-mapping-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: InstanceMapping
---
