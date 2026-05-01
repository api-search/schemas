---
description: An HTTP Live Streaming (HLS) ingest resource configuration.
layout: schema
name: HlsIngest
properties_list:
- description: ''
  name: IngestEndpoints
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-hls-ingest-schema.json
slug: mediapackage-api-hls-ingest
source_filename: mediapackage-api-hls-ingest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-ingest-schema.json\",\n  \"title\": \"HlsIngest\",\n  \"description\": \"An HTTP Live Streaming (HLS) ingest resource configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IngestEndpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfIngestEndpoint\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingestEndpoints\"\n          },\n          \"description\": \"A list of endpoints to which the source stream should be sent.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-hls-ingest-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: HlsIngest
---
