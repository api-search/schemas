---
description: The optional configuration for a server that serves segments. Use this if you want the segment delivery server to be different from the source location server. For example, you can configure your source location server to be an origination server, such as MediaPackage, and the segment delivery server to be a content delivery network (CDN), such as CloudFront. If you don't specify a segment delivery server, then the source location server is used.
layout: schema
name: DefaultSegmentDeliveryConfiguration
properties_list:
- description: ''
  name: BaseUrl
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-default-segment-delivery-configuration-schema.json
slug: mediatailor-api-default-segment-delivery-configuration
source_filename: mediatailor-api-default-segment-delivery-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-default-segment-delivery-configuration-schema.json\",\n  \"title\": \"DefaultSegmentDeliveryConfiguration\",\n  \"description\": \"The optional configuration for a server that serves segments. Use this if you want the segment delivery server to be different from the source location server. For example, you can configure your source location server to be an origination server, such as MediaPackage, and the segment delivery server to be a content delivery network (CDN), such as CloudFront. If you don't specify a segment delivery server, then the source location server is used.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BaseUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The\
  \ hostname of the server that will be used to serve segments. This string must include the protocol, such as <b>https://</b>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-default-segment-delivery-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DefaultSegmentDeliveryConfiguration
---
