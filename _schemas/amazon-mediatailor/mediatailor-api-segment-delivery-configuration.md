---
description: The segment delivery configuration settings.
layout: schema
name: SegmentDeliveryConfiguration
properties_list:
- description: ''
  name: BaseUrl
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-segment-delivery-configuration-schema.json
slug: mediatailor-api-segment-delivery-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-segment-delivery-configuration-schema.json\",\n  \"title\": \"SegmentDeliveryConfiguration\",\n  \"description\": \"The segment delivery configuration settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BaseUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The base URL of the host or path of the segment delivery server that you're using to serve segments. This is typically a content delivery network (CDN). The URL can be absolute or relative. To use an absolute URL include the protocol, such as <code>https://example.com/some/path</code>. To use a relative URL specify the relative path, such as <code>/some/path*</code>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A unique identifier used to distinguish between multiple segment delivery configurations in a source location.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-segment-delivery-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: SegmentDeliveryConfiguration
---
