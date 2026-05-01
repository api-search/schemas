---
description: '<p>A map that contains tag keys and tag values to attach to an Amazon Web Services X-Ray group or sampling rule. For more information about ways to use tags, see <a href="https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference</i>.</p> <p>The following restrictions apply to tags:</p> <ul> <li> <p>Maximum number of user-applied tags per resource: 50</p> </li> <li> <p>Tag keys and values are case sensitive.</p> </li> <li> <p>Don''t use <code>aws:</code> as a prefix for keys; it''s reserved for Amazon Web Services use. You cannot edit or delete system tags.</p> </li> </ul>'
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-tag-schema.json
slug: xray-tag
source_filename: xray-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ],\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"A tag key, such as <code>Stage</code> or <code>Name</code>. A tag key cannot be empty. The key can be a maximum of 128 characters, and can contain only Unicode letters, numbers, or separators, or the following special characters: <code>+ - = . _ : /</code> \"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n        {\n          \"description\": \"An optional tag value, such as <code>Production</code> or <code>test-only</code>. The value can be a maximum of 255 characters, and contain only Unicode letters, numbers, or separators, or the following special characters: <code>+ - = . _ : /</code> \"\n        }\n      ]\n    }\n  },\n\
  \  \"description\": \"<p>A map that contains tag keys and tag values to attach to an Amazon Web Services X-Ray group or sampling rule. For more information about ways to use tags, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference</i>.</p> <p>The following restrictions apply to tags:</p> <ul> <li> <p>Maximum number of user-applied tags per resource: 50</p> </li> <li> <p>Tag keys and values are case sensitive.</p> </li> <li> <p>Don't use <code>aws:</code> as a prefix for keys; it's reserved for Amazon Web Services use. You cannot edit or delete system tags.</p> </li> </ul>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Tag\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-tag-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-tag-schema.json
tags:
- Application Performance
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: Tag
---
