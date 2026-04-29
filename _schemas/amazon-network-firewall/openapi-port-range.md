---
description: A single port range specification. This is used for source and destination port ranges in the stateless rule <a>MatchAttributes</a>, <code>SourcePorts</code>, and <code>DestinationPorts</code> settings.
layout: schema
name: PortRange
properties_list:
- description: ''
  name: FromPort
  type: object
- description: ''
  name: ToPort
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-port-range-schema.json
slug: openapi-port-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-port-range-schema.json\",\n  \"title\": \"PortRange\",\n  \"description\": \"A single port range specification. This is used for source and destination port ranges in the stateless rule <a>MatchAttributes</a>, <code>SourcePorts</code>, and <code>DestinationPorts</code> settings. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FromPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRangeBound\"\n        },\n        {\n          \"description\": \"The lower limit of the port range. This must be less than or equal to the <code>ToPort</code> specification. \"\n        }\n      ]\n    },\n    \"ToPort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortRangeBound\"\n        },\n        {\n          \"description\"\
  : \"The upper limit of the port range. This must be greater than or equal to the <code>FromPort</code> specification. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FromPort\",\n    \"ToPort\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-port-range-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: PortRange
---
