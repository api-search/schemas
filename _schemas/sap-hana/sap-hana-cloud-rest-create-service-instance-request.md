---
description: Request body for creating a new SAP HANA Cloud service instance.
layout: schema
name: CreateServiceInstanceRequest
properties_list:
- description: The name for the new service instance. Must be unique within the subaccount.
  name: name
  type: string
- description: The service plan identifier determining the instance type and available features.
  name: service_plan_id
  type: string
- description: Labels to assign to the instance for organization and filtering.
  name: labels
  type: object
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-create-service-instance-request-schema.json
slug: sap-hana-cloud-rest-create-service-instance-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateServiceInstanceRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new SAP HANA Cloud service instance.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the new service instance. Must be unique within the subaccount.\"\n    },\n    \"service_plan_id\": {\n      \"type\": \"string\",\n      \"description\": \"The service plan identifier determining the instance type and available features.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Labels to assign to the instance for organization and filtering.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-create-service-instance-request-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: CreateServiceInstanceRequest
---
