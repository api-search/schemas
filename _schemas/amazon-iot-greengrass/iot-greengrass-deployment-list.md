---
description: DeploymentList schema
layout: schema
name: DeploymentList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-deployment-list-schema.json
slug: iot-greengrass-deployment-list
source_filename: iot-greengrass-deployment-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-list-schema.json\",\n  \"title\": \"DeploymentList\",\n  \"description\": \"DeploymentList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"targetArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/TargetARN\"\n          },\n          {\n            \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the target IoT thing or thing group. When creating a subdeployment, the targetARN can only be a thing group.\"\n          }\n        ]\n      },\n      \"revisionId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n           \
  \ \"description\": \"The revision number of the deployment.\"\n          }\n        ]\n      },\n      \"deploymentId\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The ID of the deployment.\"\n          }\n        ]\n      },\n      \"deploymentName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The name of the deployment.\"\n          }\n        ]\n      },\n      \"creationTimestamp\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The time at which the deployment was created, expressed in ISO 8601 format.\"\n          }\n        ]\n      },\n      \"deploymentStatus\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/DeploymentStatus\"\
  \n          },\n          {\n            \"description\": \"The status of the deployment.\"\n          }\n        ]\n      },\n      \"isLatestForTarget\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/IsLatestForTarget\"\n          },\n          {\n            \"description\": \"Whether or not the deployment is the latest revision for its target.\"\n          }\n        ]\n      },\n      \"parentTargetArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ThingGroupARN\"\n          },\n          {\n            \"description\": \"The parent deployment's target <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> within a subdeployment.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a deployment.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-deployment-list-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DeploymentList
---
