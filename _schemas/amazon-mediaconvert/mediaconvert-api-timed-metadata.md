---
description: 'Set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH) to include ID3 metadata in this output. This includes ID3 metadata from the following features: ID3 timestamp period (timedMetadataId3Period), and Custom ID3 metadata inserter (timedMetadataInsertion). To exclude this ID3 metadata in this output: set ID3 metadata to None (NONE) or leave blank.'
layout: schema
name: TimedMetadata
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-timed-metadata-schema.json
slug: mediaconvert-api-timed-metadata
source_filename: mediaconvert-api-timed-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timed-metadata-schema.json\",\n  \"title\": \"TimedMetadata\",\n  \"description\": \"Set ID3 metadata (timedMetadata) to Passthrough (PASSTHROUGH) to include ID3 metadata in this output. This includes ID3 metadata from the following features: ID3 timestamp period (timedMetadataId3Period), and Custom ID3 metadata inserter (timedMetadataInsertion). To exclude this ID3 metadata in this output: set ID3 metadata to None (NONE) or leave blank.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"PASSTHROUGH\",\n    \"NONE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-timed-metadata-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: TimedMetadata
---
