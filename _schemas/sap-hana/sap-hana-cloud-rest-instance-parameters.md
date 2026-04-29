---
description: Configuration parameters for an SAP HANA Cloud service instance defining resource allocation, features, and operational settings.
layout: schema
name: InstanceParameters
properties_list:
- description: The instance configuration data.
  name: data
  type: object
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-instance-parameters-schema.json
slug: sap-hana-cloud-rest-instance-parameters
source_filename: sap-hana-cloud-rest-instance-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceParameters\",\n  \"type\": \"object\",\n  \"description\": \"Configuration parameters for an SAP HANA Cloud service instance defining resource allocation, features, and operational settings.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The instance configuration data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-instance-parameters-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: InstanceParameters
---
