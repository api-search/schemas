---
description: GetApplicationResponse schema from AWS Mainframe Modernization API
layout: schema
name: GetApplicationResponse
properties_list:
- description: ''
  name: applicationArn
  type: object
- description: ''
  name: applicationId
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: deployedVersion
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: engineType
  type: object
- description: ''
  name: environmentId
  type: object
- description: ''
  name: kmsKeyId
  type: object
- description: ''
  name: lastStartTime
  type: object
- description: ''
  name: latestVersion
  type: object
- description: ''
  name: listenerArns
  type: object
- description: ''
  name: listenerPorts
  type: object
- description: ''
  name: loadBalancerDnsName
  type: object
- description: ''
  name: logGroups
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: statusReason
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: targetGroupArns
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-get-application-response-schema.json
slug: amazon-mainframe-modernization-get-application-response
source_filename: amazon-mainframe-modernization-get-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-application-response-schema.json\",\n  \"title\": \"GetApplicationResponse\",\n  \"description\": \"GetApplicationResponse schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n        }\n      ]\n    },\n    \"applicationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The identifier of the application.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when this application was created.\"\n        }\n      ]\n    },\n    \"deployedVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeployedVersionSummary\"\n        },\n        {\n          \"description\": \"The version of the application that is deployed.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityDescription\"\n        },\n        {\n          \"description\": \"The description of the application.\"\n        }\n      ]\n    },\n    \"engineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"description\": \"The type of the target platform for the application.\"\n        }\n      ]\n    },\n    \"environmentId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\
  \n        },\n        {\n          \"description\": \"The identifier of the runtime environment where you want to deploy the application.\"\n        }\n      ]\n    },\n    \"kmsKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier of a customer managed key.\"\n        }\n      ]\n    },\n    \"lastStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The timestamp when you last started the application. Null until the application runs for the first time.\"\n        }\n      ]\n    },\n    \"latestVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionSummary\"\n        },\n        {\n          \"description\": \"The latest version of the application.\"\n        }\n      ]\n    },\n    \"listenerArns\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/ArnList\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the network load balancer listener created in your Amazon Web Services account. Amazon Web Services Mainframe Modernization creates this listener for you the first time you deploy an application.\"\n        }\n      ]\n    },\n    \"listenerPorts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortList\"\n        },\n        {\n          \"description\": \"The port associated with the network load balancer listener created in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"loadBalancerDnsName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String100\"\n        },\n        {\n          \"description\": \"The public DNS name of the load balancer created in your Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"logGroups\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupSummaries\"\n        },\n        {\n          \"description\": \"The list of log summaries. Each log summary includes the log type as well as the log group identifier. These are CloudWatch logs. Amazon Web Services Mainframe Modernization pushes the application log to CloudWatch under the customer's account.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityName\"\n        },\n        {\n          \"description\": \"The unique identifier of the application.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role associated with the application.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationLifecycle\"\
  \n        },\n        {\n          \"description\": \"The status of the application.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for the reported status.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of tags associated with the application.\"\n        }\n      ]\n    },\n    \"targetGroupArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArnList\"\n        },\n        {\n          \"description\": \"Returns the Amazon Resource Names (ARNs) of the target groups that are attached to the network load balancer.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"applicationArn\",\n    \"applicationId\",\n    \"creationTime\",\n    \"engineType\",\n\
  \    \"latestVersion\",\n    \"name\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-get-application-response-schema.json
tags:
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: GetApplicationResponse
---
