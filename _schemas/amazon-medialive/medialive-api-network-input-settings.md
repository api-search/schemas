---
description: Network source to transcode. Must be accessible to the Elemental Live node that is running the live event through a network connection.
layout: schema
name: NetworkInputSettings
properties_list:
- description: ''
  name: HlsInputSettings
  type: object
- description: ''
  name: ServerValidation
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-network-input-settings-schema.json
slug: medialive-api-network-input-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-network-input-settings-schema.json\",\n  \"title\": \"NetworkInputSettings\",\n  \"description\": \"Network source to transcode. Must be accessible to the Elemental Live node that is running the live event through a network connection.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"HlsInputSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HlsInputSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hlsInputSettings\"\n          },\n          \"description\": \"Specifies HLS input settings when the uri is for a HLS manifest.\"\n        }\n      ]\n    },\n    \"ServerValidation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInputServerValidation\"\n        },\n        {\n  \
  \        \"xml\": {\n            \"name\": \"serverValidation\"\n          },\n          \"description\": \"Check HTTPS server certificates. When set to checkCryptographyOnly, cryptography in the certificate will be checked, but not the server's name. Certain subdomains (notably S3 buckets that use dots in the bucket name) do not strictly match the corresponding certificate's wildcard pattern and would otherwise cause the event to error. This setting is ignored for protocols that do not use https.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-network-input-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: NetworkInputSettings
---
