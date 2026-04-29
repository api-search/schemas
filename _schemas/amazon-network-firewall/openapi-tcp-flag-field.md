---
description: TCP flags and masks to inspect packets for, used in stateless rules <a>MatchAttributes</a> settings.
layout: schema
name: TCPFlagField
properties_list:
- description: ''
  name: Flags
  type: object
- description: ''
  name: Masks
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-tcp-flag-field-schema.json
slug: openapi-tcp-flag-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tcp-flag-field-schema.json\",\n  \"title\": \"TCPFlagField\",\n  \"description\": \"TCP flags and masks to inspect packets for, used in stateless rules <a>MatchAttributes</a> settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Flags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Flags\"\n        },\n        {\n          \"description\": \"<p>Used in conjunction with the <code>Masks</code> setting to define the flags that must be set and flags that must not be set in order for the packet to match. This setting can only specify values that are also specified in the <code>Masks</code> setting.</p> <p>For the flags that are specified in the masks setting, the following must be true for the packet to match: </p> <ul> <li> <p>The ones that are set\
  \ in this flags setting must be set in the packet. </p> </li> <li> <p>The ones that are not set in this flags setting must also not be set in the packet. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Masks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Flags\"\n        },\n        {\n          \"description\": \"The set of flags to consider in the inspection. To inspect all flags in the valid values list, leave this with no setting.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Flags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tcp-flag-field-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: TCPFlagField
---
