---
description: A metering data record representing resource consumption for billing purposes.
layout: schema
name: MeteringValue
properties_list:
- description: ISO 8601 timestamp for the metering period.
  name: timestamp
  type: string
- description: The number of compute unit hours consumed during the metering period. Compute units are based on memory and vCPU allocation.
  name: computeUnitHours
  type: number
- description: The storage consumption in gigabytes during the metering period.
  name: storageGB
  type: number
- description: The data lake storage consumption in gigabytes during the metering period, if a data lake instance is attached.
  name: dataLakeCapacityGB
  type: number
- description: The backup storage consumption in gigabytes during the metering period.
  name: backupStorageGB
  type: number
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-metering-value-schema.json
slug: sap-hana-cloud-rest-metering-value
source_filename: sap-hana-cloud-rest-metering-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeteringValue\",\n  \"type\": \"object\",\n  \"description\": \"A metering data record representing resource consumption for billing purposes.\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp for the metering period.\"\n    },\n    \"computeUnitHours\": {\n      \"type\": \"number\",\n      \"description\": \"The number of compute unit hours consumed during the metering period. Compute units are based on memory and vCPU allocation.\"\n    },\n    \"storageGB\": {\n      \"type\": \"number\",\n      \"description\": \"The storage consumption in gigabytes during the metering period.\"\n    },\n    \"dataLakeCapacityGB\": {\n      \"type\": \"number\",\n      \"description\": \"The data lake storage consumption in gigabytes during the metering period, if a data lake instance is attached.\"\n    },\n    \"backupStorageGB\": {\n\
  \      \"type\": \"number\",\n      \"description\": \"The backup storage consumption in gigabytes during the metering period.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-metering-value-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: MeteringValue
---
