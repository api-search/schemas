---
description: EndpointString schema from Amazon EventBridge Pipes
layout: schema
name: EndpointString
properties_list: []
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-endpoint-string-schema.json
slug: amazon-eventbridge-pipes-endpoint-string
source_filename: amazon-eventbridge-pipes-endpoint-string-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-endpoint-string-schema.json\",\n  \"title\": \"EndpointString\",\n  \"description\": \"EndpointString schema from Amazon EventBridge Pipes\",\n  \"type\": \"string\",\n  \"format\": \"password\",\n  \"pattern\": \"^(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\\\\-]*[a-zA-Z0-9])\\\\.)*([A-Za-z0-9]|[A-Za-z0-9][A-Za-z0-9\\\\-]*[A-Za-z0-9]):[0-9]{1,5}$\",\n  \"minLength\": 1,\n  \"maxLength\": 300\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-endpoint-string-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: EndpointString
---
