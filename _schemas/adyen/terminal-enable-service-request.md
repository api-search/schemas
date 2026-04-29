---
description: It conveys the services that will be enabled for the POI Terminal without the request of the Sale System, and a possible invitation for the Customer to start the services. Content of the Enable Service Request message.
layout: schema
name: EnableServiceRequest
properties_list:
- description: ''
  name: TransactionAction
  type: object
- description: ''
  name: ServicesEnabled
  type: object
- description: ''
  name: DisplayOutput
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-enable-service-request-schema.json
slug: terminal-enable-service-request
source_filename: terminal-enable-service-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-enable-service-request-schema.json\",\n  \"title\": \"EnableServiceRequest\",\n  \"description\": \"It conveys the services that will be enabled for the  POI Terminal without the request of the Sale System, and a possible invitation for the Customer to start the services. Content of the Enable Service Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactionAction\": {\n      \"$ref\": \"#/components/schemas/TransactionAction\"\n    },\n    \"ServicesEnabled\": {\n      \"$ref\": \"#/components/schemas/ServicesEnabled\"\n    },\n    \"DisplayOutput\": {\n      \"$ref\": \"#/components/schemas/DisplayOutput\"\n    }\n  },\n  \"required\": [\n    \"TransactionAction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-enable-service-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EnableServiceRequest
---
