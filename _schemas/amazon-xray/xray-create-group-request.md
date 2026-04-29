---
description: CreateGroupRequest schema from Amazon X-Ray API
layout: schema
name: CreateGroupRequest
properties_list:
- description: ''
  name: GroupName
  type: object
- description: ''
  name: FilterExpression
  type: object
- description: ''
  name: InsightsConfiguration
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-create-group-request-schema.json
slug: xray-create-group-request
source_filename: xray-create-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"GroupName\"\n  ],\n  \"title\": \"CreateGroupRequest\",\n  \"properties\": {\n    \"GroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupName\"\n        },\n        {\n          \"description\": \"The case-sensitive name of the new group. Default is a reserved name and names must be unique.\"\n        }\n      ]\n    },\n    \"FilterExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterExpression\"\n        },\n        {\n          \"description\": \"The filter expression defining criteria by which to group traces.\"\n        }\n      ]\n    },\n    \"InsightsConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightsConfiguration\"\n        },\n        {\n          \"description\": \"<p>The structure containing configurations related to insights.</p> <ul> <li> <p>The InsightsEnabled boolean can\
  \ be set to true to enable insights for the new group or false to disable insights for the new group.</p> </li> <li> <p>The NotificationsEnabled boolean can be set to true to enable insights notifications for the new group. Notifications may only be enabled on a group with InsightsEnabled set to true.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>A map that contains one or more tag keys and tag values to attach to an X-Ray group. For more information about ways to use tags, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference</i>.</p> <p>The following restrictions apply to tags:</p> <ul> <li> <p>Maximum number of user-applied tags per resource: 50</p> </li> <li> <p>Maximum tag key length: 128 Unicode characters</p>\
  \ </li> <li> <p>Maximum tag value length: 256 Unicode characters</p> </li> <li> <p>Valid values for key and value: a-z, A-Z, 0-9, space, and the following characters: _ . : / = + - and @</p> </li> <li> <p>Tag keys and values are case sensitive.</p> </li> <li> <p>Don't use <code>aws:</code> as a prefix for keys; it's reserved for Amazon Web Services use.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-create-group-request-schema.json\",\n  \"description\": \"CreateGroupRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-create-group-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: CreateGroupRequest
---
