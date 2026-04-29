---
description: The configuration and status for a single subnet that you've specified for use by the Network Firewall firewall. This is part of the <a>FirewallStatus</a>.
layout: schema
name: Attachment
properties_list:
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: EndpointId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-attachment-schema.json
slug: openapi-attachment
source_filename: openapi-attachment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-attachment-schema.json\",\n  \"title\": \"Attachment\",\n  \"description\": \"The configuration and status for a single subnet that you've specified for use by the Network Firewall firewall. This is part of the <a>FirewallStatus</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AzSubnet\"\n        },\n        {\n          \"description\": \"The unique identifier of the subnet that you've specified to be used for a firewall endpoint. \"\n        }\n      ]\n    },\n    \"EndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointId\"\n        },\n        {\n          \"description\": \"The identifier of the firewall endpoint that Network Firewall has\
  \ instantiated in the subnet. You use this to identify the firewall endpoint in the VPC route tables, when you redirect the VPC traffic through the endpoint. \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttachmentStatus\"\n        },\n        {\n          \"description\": \"The current status of the firewall endpoint in the subnet. This value reflects both the instantiation of the endpoint in the VPC subnet and the sync states that are reported in the <code>Config</code> settings. When this value is <code>READY</code>, the endpoint is available and configured properly to handle network traffic. When the endpoint isn't available for traffic, this value will reflect its state, for example <code>CREATING</code> or <code>DELETING</code>.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusMessage\"\n        },\n        {\n    \
  \      \"description\": \"If Network Firewall fails to create or delete the firewall endpoint in the subnet, it populates this with the reason for the failure and how to resolve it. Depending on the error, it can take as many as 15 minutes to populate this field. For more information about the errors and solutions available for this field, see <a href=\\\"https://docs.aws.amazon.com/network-firewall/latest/developerguide/firewall-troubleshooting-endpoint-failures.html\\\">Troubleshooting firewall endpoint failures</a> in the <i>Network Firewall Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-attachment-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: Attachment
---
