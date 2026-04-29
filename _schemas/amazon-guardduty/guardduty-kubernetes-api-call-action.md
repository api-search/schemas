---
description: Information about the Kubernetes API call action described in this finding.
layout: schema
name: KubernetesApiCallAction
properties_list:
- description: ''
  name: RequestUri
  type: object
- description: ''
  name: Verb
  type: object
- description: ''
  name: SourceIps
  type: object
- description: ''
  name: UserAgent
  type: object
- description: ''
  name: RemoteIpDetails
  type: object
- description: ''
  name: StatusCode
  type: object
- description: ''
  name: Parameters
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-kubernetes-api-call-action-schema.json
slug: guardduty-kubernetes-api-call-action
source_filename: guardduty-kubernetes-api-call-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-api-call-action-schema.json\",\n  \"title\": \"KubernetesApiCallAction\",\n  \"description\": \"Information about the Kubernetes API call action described in this finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"requestUri\"\n          },\n          \"description\": \"The Kubernetes API request URI.\"\n        }\n      ]\n    },\n    \"Verb\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"verb\"\n          },\n          \"description\": \"The Kubernetes API request HTTP verb.\"\n        }\n\
  \      ]\n    },\n    \"SourceIps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceIps\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceIps\"\n          },\n          \"description\": \"The IP of the Kubernetes API caller and the IPs of any proxies or load balancers between the caller and the API endpoint.\"\n        }\n      ]\n    },\n    \"UserAgent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userAgent\"\n          },\n          \"description\": \"The user agent of the caller of the Kubernetes API.\"\n        }\n      ]\n    },\n    \"RemoteIpDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteIpDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteIpDetails\"\n          }\n        }\n      ]\n    },\n    \"StatusCode\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"statusCode\"\n          },\n          \"description\": \"The resulting HTTP response code of the Kubernetes API call action.\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"parameters\"\n          },\n          \"description\": \"Parameters related to the Kubernetes API call action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-kubernetes-api-call-action-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: KubernetesApiCallAction
---
