---
description: The parameters required to set up enrichment on your pipe.
layout: schema
name: PipeEnrichmentParameters
properties_list:
- description: ''
  name: HttpParameters
  type: object
- description: ''
  name: InputTemplate
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-enrichment-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-enrichment-parameters
source_filename: amazon-eventbridge-pipes-pipe-enrichment-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-enrichment-parameters-schema.json\",\n  \"title\": \"PipeEnrichmentParameters\",\n  \"description\": \"The parameters required to set up enrichment on your pipe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeEnrichmentHttpParameters\"\n        },\n        {\n          \"description\": \"<p>Contains the HTTP parameters to use when the target is a API Gateway REST endpoint or EventBridge ApiDestination.</p> <p>If you specify an API Gateway REST API or EventBridge ApiDestination as a target, you can use this parameter to specify headers, path parameters, and query string keys/values as part of your target invoking request. If you're using ApiDestinations, the\
  \ corresponding Connection can also have these values configured. In case of any conflicting keys, values from the Connection take precedence.</p>\"\n        }\n      ]\n    },\n    \"InputTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTemplate\"\n        },\n        {\n          \"description\": \"Valid JSON text passed to the enrichment. In this case, nothing from the event itself is passed to the enrichment. For more information, see <a href=\\\"http://www.rfc-editor.org/rfc/rfc7159.txt\\\">The JavaScript Object Notation (JSON) Data Interchange Format</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-enrichment-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeEnrichmentParameters
---
