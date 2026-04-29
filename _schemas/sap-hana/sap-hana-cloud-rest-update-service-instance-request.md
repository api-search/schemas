---
description: Request body for updating an existing SAP HANA Cloud service instance. Only include the parameters that need to be changed.
layout: schema
name: UpdateServiceInstanceRequest
properties_list:
- description: The updated name for the service instance.
  name: name
  type: string
- description: Updated labels for the service instance.
  name: labels
  type: object
- description: The new service plan identifier if changing the instance plan.
  name: service_plan_id
  type: string
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-update-service-instance-request-schema.json
slug: sap-hana-cloud-rest-update-service-instance-request
source_filename: sap-hana-cloud-rest-update-service-instance-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateServiceInstanceRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an existing SAP HANA Cloud service instance. Only include the parameters that need to be changed.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The updated name for the service instance.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Updated labels for the service instance.\"\n    },\n    \"service_plan_id\": {\n      \"type\": \"string\",\n      \"description\": \"The new service plan identifier if changing the instance plan.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-update-service-instance-request-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: UpdateServiceInstanceRequest
---
