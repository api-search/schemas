---
description: Standard error response returned by the SAP HANA Cloud REST API when a request fails.
layout: schema
name: Error
properties_list:
- description: The error code identifying the type of error.
  name: error
  type: string
- description: A human-readable description of the error.
  name: description
  type: string
- description: The HTTP status code associated with the error.
  name: statusCode
  type: integer
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-error-schema.json
slug: sap-hana-cloud-rest-error
source_filename: sap-hana-cloud-rest-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response returned by the SAP HANA Cloud REST API when a request fails.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"The error code identifying the type of error.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    },\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code associated with the error.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-error-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: Error
---
