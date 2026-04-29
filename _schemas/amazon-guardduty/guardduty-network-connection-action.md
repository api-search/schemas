---
description: Contains information about the NETWORK_CONNECTION action described in the finding.
layout: schema
name: NetworkConnectionAction
properties_list:
- description: ''
  name: Blocked
  type: object
- description: ''
  name: ConnectionDirection
  type: object
- description: ''
  name: LocalPortDetails
  type: object
- description: ''
  name: Protocol
  type: object
- description: ''
  name: LocalIpDetails
  type: object
- description: ''
  name: RemoteIpDetails
  type: object
- description: ''
  name: RemotePortDetails
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-network-connection-action-schema.json
slug: guardduty-network-connection-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-network-connection-action-schema.json\",\n  \"title\": \"NetworkConnectionAction\",\n  \"description\": \"Contains information about the NETWORK_CONNECTION action described in the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Blocked\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"blocked\"\n          },\n          \"description\": \"Indicates whether EC2 blocked the network connection to your instance.\"\n        }\n      ]\n    },\n    \"ConnectionDirection\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"connectionDirection\"\n          },\n          \"\
  description\": \"The network connection direction.\"\n        }\n      ]\n    },\n    \"LocalPortDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocalPortDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"localPortDetails\"\n          },\n          \"description\": \"The local port information of the connection.\"\n        }\n      ]\n    },\n    \"Protocol\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"protocol\"\n          },\n          \"description\": \"The network connection protocol.\"\n        }\n      ]\n    },\n    \"LocalIpDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocalIpDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"localIpDetails\"\n          },\n          \"description\": \"The local IP information of the connection.\"\
  \n        }\n      ]\n    },\n    \"RemoteIpDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteIpDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteIpDetails\"\n          },\n          \"description\": \"The remote IP information of the connection.\"\n        }\n      ]\n    },\n    \"RemotePortDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemotePortDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remotePortDetails\"\n          },\n          \"description\": \"The remote port information of the connection.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-network-connection-action-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: NetworkConnectionAction
---
