---
description: Contains information about the API action.
layout: schema
name: AwsApiCallAction
properties_list:
- description: ''
  name: Api
  type: object
- description: ''
  name: CallerType
  type: object
- description: ''
  name: DomainDetails
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: UserAgent
  type: object
- description: ''
  name: RemoteIpDetails
  type: object
- description: ''
  name: ServiceName
  type: object
- description: ''
  name: RemoteAccountDetails
  type: object
- description: ''
  name: AffectedResources
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-aws-api-call-action-schema.json
slug: guardduty-aws-api-call-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-aws-api-call-action-schema.json\",\n  \"title\": \"AwsApiCallAction\",\n  \"description\": \"Contains information about the API action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Api\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"api\"\n          },\n          \"description\": \"The Amazon Web Services API name.\"\n        }\n      ]\n    },\n    \"CallerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"callerType\"\n          },\n          \"description\": \"The Amazon Web Services API caller type.\"\n        }\n      ]\n    },\n    \"DomainDetails\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"domainDetails\"\n          },\n          \"description\": \"The domain information for the Amazon Web Services API call.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorCode\"\n          },\n          \"description\": \"The error code of the failed Amazon Web Services API action.\"\n        }\n      ]\n    },\n    \"UserAgent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"userAgent\"\n          },\n          \"description\": \"The agent through which the API request was made.\"\n        }\n      ]\n    },\n    \"RemoteIpDetails\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/RemoteIpDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteIpDetails\"\n          },\n          \"description\": \"The remote IP information of the connection that initiated the Amazon Web Services API call.\"\n        }\n      ]\n    },\n    \"ServiceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serviceName\"\n          },\n          \"description\": \"The Amazon Web Services service name whose API was invoked.\"\n        }\n      ]\n    },\n    \"RemoteAccountDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteAccountDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"remoteAccountDetails\"\n          },\n          \"description\": \"The details of the Amazon Web Services account that made the API call. This field\
  \ appears if the call was made from outside your account.\"\n        }\n      ]\n    },\n    \"AffectedResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AffectedResources\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"affectedResources\"\n          },\n          \"description\": \"The details of the Amazon Web Services account that made the API call. This field identifies the resources that were affected by this API call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-aws-api-call-action-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: AwsApiCallAction
---
