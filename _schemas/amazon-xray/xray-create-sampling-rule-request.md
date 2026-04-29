---
description: CreateSamplingRuleRequest schema from Amazon X-Ray API
layout: schema
name: CreateSamplingRuleRequest
properties_list:
- description: ''
  name: SamplingRule
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-create-sampling-rule-request-schema.json
slug: xray-create-sampling-rule-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"SamplingRule\"\n  ],\n  \"title\": \"CreateSamplingRuleRequest\",\n  \"properties\": {\n    \"SamplingRule\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamplingRule\"\n        },\n        {\n          \"description\": \"The rule definition.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>A map that contains one or more tag keys and tag values to attach to an X-Ray sampling rule. For more information about ways to use tags, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference</i>.</p> <p>The following restrictions apply to tags:</p> <ul> <li> <p>Maximum number of user-applied tags per resource: 50</p> </li> <li> <p>Maximum tag key length:\
  \ 128 Unicode characters</p> </li> <li> <p>Maximum tag value length: 256 Unicode characters</p> </li> <li> <p>Valid values for key and value: a-z, A-Z, 0-9, space, and the following characters: _ . : / = + - and @</p> </li> <li> <p>Tag keys and values are case sensitive.</p> </li> <li> <p>Don't use <code>aws:</code> as a prefix for keys; it's reserved for Amazon Web Services use.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-create-sampling-rule-request-schema.json\",\n  \"description\": \"CreateSamplingRuleRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-create-sampling-rule-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: CreateSamplingRuleRequest
---
