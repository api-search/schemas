---
description: The configuration for DASH PUT operations.
layout: schema
name: DashConfigurationForPut
properties_list:
- description: ''
  name: MpdLocation
  type: object
- description: ''
  name: OriginManifestType
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-dash-configuration-for-put-schema.json
slug: mediatailor-api-dash-configuration-for-put
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-dash-configuration-for-put-schema.json\",\n  \"title\": \"DashConfigurationForPut\",\n  \"description\": \"The configuration for DASH PUT operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MpdLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The setting that controls whether MediaTailor includes the Location tag in DASH manifests. MediaTailor populates the Location tag with the URL for manifest update requests, to be used by players that don't support sticky redirects. Disable this if you have CDN routing rules set up for accessing MediaTailor manifests, and you are either using client-side reporting or your players support sticky HTTP redirects. Valid values are <code>DISABLED</code>\
  \ and <code>EMT_DEFAULT</code>. The <code>EMT_DEFAULT</code> setting enables the inclusion of the tag and is the default value.\"\n        }\n      ]\n    },\n    \"OriginManifestType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OriginManifestType\"\n        },\n        {\n          \"description\": \"The setting that controls whether MediaTailor handles manifests from the origin server as multi-period manifests or single-period manifests. If your origin server produces single-period manifests, set this to <code>SINGLE_PERIOD</code>. The default setting is <code>MULTI_PERIOD</code>. For multi-period manifests, omit this setting or set it to <code>MULTI_PERIOD</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-dash-configuration-for-put-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DashConfigurationForPut
---
