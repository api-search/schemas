---
description: If your output group type is HLS, DASH, or Microsoft Smooth, use these settings when doing DRM encryption with a SPEKE-compliant key provider. If your output group type is CMAF, use the SpekeKeyProviderCmaf settings instead.
layout: schema
name: SpekeKeyProvider
properties_list:
- description: ''
  name: CertificateArn
  type: object
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: SystemIds
  type: object
- description: ''
  name: Url
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-speke-key-provider-schema.json
slug: mediaconvert-api-speke-key-provider
source_filename: mediaconvert-api-speke-key-provider-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-speke-key-provider-schema.json\",\n  \"title\": \"SpekeKeyProvider\",\n  \"description\": \"If your output group type is HLS, DASH, or Microsoft Smooth, use these settings when doing DRM encryption with a SPEKE-compliant key provider. If your output group type is CMAF, use the SpekeKeyProviderCmaf settings instead.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternArnAwsUsGovAcm\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"certificateArn\"\n          },\n          \"description\": \"If you want your key provider to encrypt the content keys that it provides to MediaConvert, set up a certificate with a master key using AWS Certificate Manager.\
  \ Specify the certificate's Amazon Resource Name (ARN) here.\"\n        }\n      ]\n    },\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resourceId\"\n          },\n          \"description\": \"Specify the resource ID that your SPEKE-compliant key provider uses to identify this content.\"\n        }\n      ]\n    },\n    \"SystemIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__stringPattern09aFAF809aFAF409aFAF409aFAF409aFAF12\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"systemIds\"\n          },\n          \"description\": \"Relates to SPEKE implementation. DRM system identifiers. DASH output groups support a max of two system ids. Other group types support one system id. See\\n https://dashif.org/identifiers/content_protection/ for more details.\"\n        }\n      ]\n    },\n    \"\
  Url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternHttps\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"url\"\n          },\n          \"description\": \"Specify the URL to the key server that your SPEKE-compliant DRM key provider uses to provide keys for encrypting your content.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-speke-key-provider-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: SpekeKeyProvider
---
