---
description: Contains information about actions.
layout: schema
name: Action
properties_list:
- description: ''
  name: ActionType
  type: object
- description: ''
  name: AwsApiCallAction
  type: object
- description: ''
  name: DnsRequestAction
  type: object
- description: ''
  name: NetworkConnectionAction
  type: object
- description: ''
  name: PortProbeAction
  type: object
- description: ''
  name: KubernetesApiCallAction
  type: object
- description: ''
  name: RdsLoginAttemptAction
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-action-schema.json
slug: guardduty-action
source_filename: guardduty-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"Contains information about actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"actionType\"\n          },\n          \"description\": \"The GuardDuty finding activity type.\"\n        }\n      ]\n    },\n    \"AwsApiCallAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsApiCallAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"awsApiCallAction\"\n          },\n          \"description\": \"Information about the AWS_API_CALL action described in this finding.\"\n        }\n      ]\n\
  \    },\n    \"DnsRequestAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsRequestAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"dnsRequestAction\"\n          },\n          \"description\": \"Information about the DNS_REQUEST action described in this finding.\"\n        }\n      ]\n    },\n    \"NetworkConnectionAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkConnectionAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkConnectionAction\"\n          },\n          \"description\": \"Information about the NETWORK_CONNECTION action described in this finding.\"\n        }\n      ]\n    },\n    \"PortProbeAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortProbeAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"portProbeAction\"\n          },\n          \"description\": \"Information\
  \ about the PORT_PROBE action described in this finding.\"\n        }\n      ]\n    },\n    \"KubernetesApiCallAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KubernetesApiCallAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"kubernetesApiCallAction\"\n          },\n          \"description\": \"Information about the Kubernetes API call action described in this finding.\"\n        }\n      ]\n    },\n    \"RdsLoginAttemptAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RdsLoginAttemptAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"rdsLoginAttemptAction\"\n          },\n          \"description\": \"Information about <code>RDS_LOGIN_ATTEMPT</code> action described in this finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-action-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Action
---
