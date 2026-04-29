---
description: An SAP HANA Cloud instance as represented in the inventory service, providing a consolidated view of instance status and configuration.
layout: schema
name: InventoryInstance
properties_list:
- description: The unique identifier of the service instance.
  name: serviceInstanceId
  type: string
- description: The name of the service plan (e.g., hana, hana-td, relational-data-lake).
  name: servicePlanName
  type: string
- description: The display name of the instance.
  name: instanceName
  type: string
- description: The current provisioning state of the instance.
  name: provisioningState
  type: string
- description: The current operational state of the instance.
  name: operationalState
  type: string
- description: Allocated memory in gigabytes.
  name: memory
  type: integer
- description: Number of allocated virtual CPUs.
  name: vcpu
  type: integer
- description: Allocated persistent storage in gigabytes.
  name: storage
  type: integer
- description: ISO 8601 timestamp when the instance was created.
  name: createdAt
  type: string
- description: ISO 8601 timestamp when the instance was last modified.
  name: modifiedAt
  type: string
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-inventory-instance-schema.json
slug: sap-hana-cloud-rest-inventory-instance
source_filename: sap-hana-cloud-rest-inventory-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryInstance\",\n  \"type\": \"object\",\n  \"description\": \"An SAP HANA Cloud instance as represented in the inventory service, providing a consolidated view of instance status and configuration.\",\n  \"properties\": {\n    \"serviceInstanceId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the service instance.\"\n    },\n    \"servicePlanName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service plan (e.g., hana, hana-td, relational-data-lake).\"\n    },\n    \"instanceName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the instance.\"\n    },\n    \"provisioningState\": {\n      \"type\": \"string\",\n      \"description\": \"The current provisioning state of the instance.\"\n    },\n    \"operationalState\": {\n      \"type\": \"string\",\n      \"description\": \"The current operational\
  \ state of the instance.\"\n    },\n    \"memory\": {\n      \"type\": \"integer\",\n      \"description\": \"Allocated memory in gigabytes.\"\n    },\n    \"vcpu\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of allocated virtual CPUs.\"\n    },\n    \"storage\": {\n      \"type\": \"integer\",\n      \"description\": \"Allocated persistent storage in gigabytes.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the instance was created.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp when the instance was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-inventory-instance-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: InventoryInstance
---
