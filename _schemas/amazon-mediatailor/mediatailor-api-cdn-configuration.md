---
description: The configuration for using a content delivery network (CDN), like Amazon CloudFront, for content and ad segment management.
layout: schema
name: CdnConfiguration
properties_list:
- description: ''
  name: AdSegmentUrlPrefix
  type: object
- description: ''
  name: ContentSegmentUrlPrefix
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-cdn-configuration-schema.json
slug: mediatailor-api-cdn-configuration
source_filename: mediatailor-api-cdn-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-cdn-configuration-schema.json\",\n  \"title\": \"CdnConfiguration\",\n  \"description\": \"The configuration for using a content delivery network (CDN), like Amazon CloudFront, for content and ad segment management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdSegmentUrlPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A non-default content delivery network (CDN) to serve ad segments. By default, AWS Elemental MediaTailor uses Amazon CloudFront with default cache settings as its CDN for ad segments. To set up an alternate CDN, create a rule in your CDN for the origin ads.mediatailor.<i>&lt;region&gt;</i>.amazonaws.com. Then specify the rule's name in this <code>AdSegmentUrlPrefix</code>.\
  \ When AWS Elemental MediaTailor serves a manifest, it reports your CDN as the source for ad segments.\"\n        }\n      ]\n    },\n    \"ContentSegmentUrlPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"A content delivery network (CDN) to cache content segments, so that content requests don\\u2019t always have to go to the origin server. First, create a rule in your CDN for the content segment origin server. Then specify the rule's name in this <code>ContentSegmentUrlPrefix</code>. When AWS Elemental MediaTailor serves a manifest, it reports your CDN as the source for content segments.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-cdn-configuration-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: CdnConfiguration
---
