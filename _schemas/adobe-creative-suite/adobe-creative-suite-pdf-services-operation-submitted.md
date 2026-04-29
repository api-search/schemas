---
description: Response returned when an operation has been accepted
layout: schema
name: OperationSubmitted
properties_list:
- description: Unique identifier for the submitted operation job
  name: jobID
  type: string
provider_name: Adobe Creative Suite
provider_slug: adobe-creative-suite
schema_file: json-schema/adobe-creative-suite-pdf-services-operation-submitted-schema.json
slug: adobe-creative-suite-pdf-services-operation-submitted
source_filename: adobe-creative-suite-pdf-services-operation-submitted-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-operation-submitted-schema.json\",\n  \"title\": \"OperationSubmitted\",\n  \"description\": \"Response returned when an operation has been accepted\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the submitted operation job\",\n      \"example\": \"urn:aaid:AS:UE1:operation:abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-creative-suite/refs/heads/main/json-schema/adobe-creative-suite-pdf-services-operation-submitted-schema.json
tags:
- Creative
- Design
- Graphics
- Photography
- Video
title: OperationSubmitted
---
