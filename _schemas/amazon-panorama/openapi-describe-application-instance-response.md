---
description: DescribeApplicationInstanceResponse schema from Amazon Panorama
layout: schema
name: DescribeApplicationInstanceResponse
properties_list:
- description: ''
  name: ApplicationInstanceId
  type: object
- description: ''
  name: ApplicationInstanceIdToReplace
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreatedTime
  type: object
- description: ''
  name: DefaultRuntimeContextDevice
  type: object
- description: ''
  name: DefaultRuntimeContextDeviceName
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: HealthStatus
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RuntimeContextStates
  type: object
- description: ''
  name: RuntimeRoleArn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusDescription
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-application-instance-response-schema.json
slug: openapi-describe-application-instance-response
source_filename: openapi-describe-application-instance-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-application-instance-response-schema.json\",\n  \"title\": \"DescribeApplicationInstanceResponse\",\n  \"description\": \"DescribeApplicationInstanceResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceId\"\n        },\n        {\n          \"description\": \"The application instance's ID.\"\n        }\n      ]\n    },\n    \"ApplicationInstanceIdToReplace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceId\"\n        },\n        {\n          \"description\": \"The ID of the application instance that this instance replaced.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceArn\"\n        },\n        {\n          \"description\": \"The application instance's ARN.\"\n        }\n      ]\n    },\n    \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"When the application instance was created.\"\n        }\n      ]\n    },\n    \"DefaultRuntimeContextDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultRuntimeContextDevice\"\n        },\n        {\n          \"description\": \"The device's ID.\"\n        }\n      ]\n    },\n    \"DefaultRuntimeContextDeviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceName\"\n        },\n        {\n          \"description\": \"The device's bane.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The application instance's description.\"\n        }\n      ]\n    },\n    \"HealthStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceHealthStatus\"\n        },\n        {\n          \"description\": \"The application instance's health status.\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"The application instance was updated.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceName\"\n        },\n        {\n          \"description\": \"The application instance's name.\"\n        }\n      ]\n    },\n    \"RuntimeContextStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportedRuntimeContextStates\"\
  \n        },\n        {\n          \"description\": \"The application instance's state.\"\n        }\n      ]\n    },\n    \"RuntimeRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeRoleArn\"\n        },\n        {\n          \"description\": \"The application instance's runtime role ARN.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceStatus\"\n        },\n        {\n          \"description\": \"The application instance's status.\"\n        }\n      ]\n    },\n    \"StatusDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceStatusDescription\"\n        },\n        {\n          \"description\": \"The application instance's status description.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n      \
  \  {\n          \"description\": \"The application instance's tags.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-application-instance-response-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribeApplicationInstanceResponse
---
