---
description: UpdateLiveSourceRequest schema from Amazon MediaTailor API
layout: schema
name: UpdateLiveSourceRequest
properties_list:
- description: ''
  name: HttpPackageConfigurations
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-update-live-source-request-schema.json
slug: mediatailor-api-update-live-source-request
source_filename: mediatailor-api-update-live-source-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-live-source-request-schema.json\",\n  \"title\": \"UpdateLiveSourceRequest\",\n  \"description\": \"UpdateLiveSourceRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HttpPackageConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpPackageConfigurations\"\n        },\n        {\n          \"description\": \"A list of HTTP package configurations for the live source on this account.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"HttpPackageConfigurations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-update-live-source-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateLiveSourceRequest
---
