---
description: Rtmp Output Settings
layout: schema
name: RtmpOutputSettings
properties_list:
- description: ''
  name: CertificateMode
  type: object
- description: ''
  name: ConnectionRetryInterval
  type: object
- description: ''
  name: Destination
  type: object
- description: ''
  name: NumRetries
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-rtmp-output-settings-schema.json
slug: medialive-api-rtmp-output-settings
source_filename: medialive-api-rtmp-output-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-rtmp-output-settings-schema.json\",\n  \"title\": \"RtmpOutputSettings\",\n  \"description\": \"Rtmp Output Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RtmpOutputCertificateMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"certificateMode\"\n          },\n          \"description\": \"If set to verifyAuthenticity, verify the tls certificate chain to a trusted Certificate Authority (CA).  This will cause rtmps outputs with self-signed certificates to fail.\"\n        }\n      ]\n    },\n    \"ConnectionRetryInterval\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"connectionRetryInterval\"\n          },\n          \"description\": \"Number of seconds to wait before retrying a connection to the Flash Media server if the connection is lost.\"\n        }\n      ]\n    },\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocationRef\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destination\"\n          },\n          \"description\": \"The RTMP endpoint excluding the stream name (eg. rtmp://host/appname). For connection to Akamai, a username and password must be supplied. URI fields accept format identifiers.\"\n        }\n      ]\n    },\n    \"NumRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"numRetries\"\n          },\n          \"description\": \"Number of retry attempts.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Destination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-rtmp-output-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: RtmpOutputSettings
---
