---
description: A Cloud NGFW firewall instance deployed in an AWS VPC.
layout: schema
name: Firewall
properties_list:
- description: ''
  name: FirewallName
  type: string
- description: ''
  name: FirewallEntry
  type: object
- description: ''
  name: FirewallStatus
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-ngfw-api-firewall-schema.json
slug: cloud-ngfw-api-firewall
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Firewall\",\n  \"description\": \"A Cloud NGFW firewall instance deployed in an AWS VPC.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-firewall-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FirewallName\": {\n      \"type\": \"string\"\n    },\n    \"FirewallEntry\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Description\": {\n          \"type\": \"string\"\n        },\n        \"VpcId\": {\n          \"type\": \"string\",\n          \"description\": \"AWS VPC ID where the firewall is deployed.\"\n        },\n        \"AssociatedRuleStack\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the rule stack associated with this firewall.\"\n        },\n        \"SubnetMappings\": {\n          \"type\": \"array\",\n          \"items\": {\n      \
  \      \"type\": \"object\",\n            \"properties\": {\n              \"SubnetId\": {\n                \"type\": \"string\",\n                \"description\": \"AWS subnet ID for the firewall endpoint.\"\n              },\n              \"AvailabilityZone\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"Tags\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Key\": {\n                \"type\": \"string\"\n              },\n              \"Value\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"FirewallStatus\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"FirewallStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"PROVISIONING\",\n            \"ACTIVE\",\n            \"DELETING\",\n            \"FAILED\"\n\
  \          ]\n        },\n        \"Attachments\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"SubnetId\": {\n                \"type\": \"string\"\n              },\n              \"EndpointId\": {\n                \"type\": \"string\"\n              },\n              \"Status\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-ngfw-api-firewall-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Firewall
---
