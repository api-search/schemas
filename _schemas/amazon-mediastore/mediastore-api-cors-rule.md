---
description: A rule for a CORS policy. You can add up to 100 rules to a CORS policy. If more than one rule applies, the service uses the first applicable rule listed.
layout: schema
name: CorsRule
properties_list:
- description: ''
  name: AllowedOrigins
  type: object
- description: ''
  name: AllowedMethods
  type: object
- description: ''
  name: AllowedHeaders
  type: object
- description: ''
  name: MaxAgeSeconds
  type: object
- description: ''
  name: ExposeHeaders
  type: object
provider_name: Amazon MediaStore
provider_slug: amazon-mediastore
schema_file: json-schema/mediastore-api-cors-rule-schema.json
slug: mediastore-api-cors-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-cors-rule-schema.json\",\n  \"title\": \"CorsRule\",\n  \"description\": \"A rule for a CORS policy. You can add up to 100 rules to a CORS policy. If more than one rule applies, the service uses the first applicable rule listed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AllowedOrigins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowedOrigins\"\n        },\n        {\n          \"description\": \"<p>One or more response headers that you want users to be able to access from their applications (for example, from a JavaScript <code>XMLHttpRequest</code> object).</p> <p>Each CORS rule must have at least one <code>AllowedOrigins</code> element. The string value can include only one wildcard character (*), for example, http://*.example.com. Additionally,\
  \ you can specify only one wildcard character to allow cross-origin access for all origins.</p>\"\n        }\n      ]\n    },\n    \"AllowedMethods\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowedMethods\"\n        },\n        {\n          \"description\": \"<p>Identifies an HTTP method that the origin that is specified in the rule is allowed to execute.</p> <p>Each CORS rule must contain at least one <code>AllowedMethods</code> and one <code>AllowedOrigins</code> element.</p>\"\n        }\n      ]\n    },\n    \"AllowedHeaders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowedHeaders\"\n        },\n        {\n          \"description\": \"<p>Specifies which headers are allowed in a preflight <code>OPTIONS</code> request through the <code>Access-Control-Request-Headers</code> header. Each header name that is specified in <code>Access-Control-Request-Headers</code> must have a corresponding entry in the rule. Only\
  \ the headers that were requested are sent back. </p> <p>This element can contain only one wildcard character (*).</p>\"\n        }\n      ]\n    },\n    \"MaxAgeSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxAgeSeconds\"\n        },\n        {\n          \"description\": \"<p>The time in seconds that your browser caches the preflight response for the specified resource.</p> <p>A CORS rule can have only one <code>MaxAgeSeconds</code> element.</p>\"\n        }\n      ]\n    },\n    \"ExposeHeaders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExposeHeaders\"\n        },\n        {\n          \"description\": \"<p>One or more headers in the response that you want users to be able to access from their applications (for example, from a JavaScript <code>XMLHttpRequest</code> object).</p> <p>This element is optional for each rule.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AllowedOrigins\",\n\
  \    \"AllowedHeaders\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediastore/refs/heads/main/json-schema/mediastore-api-cors-rule-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CorsRule
---
