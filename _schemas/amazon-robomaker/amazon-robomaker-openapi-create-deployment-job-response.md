---
description: AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.
layout: schema
name: CreateDeploymentJobResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: fleet
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: deploymentApplicationConfigs
  type: object
- description: ''
  name: failureReason
  type: object
- description: ''
  name: failureCode
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: deploymentConfig
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-create-deployment-job-response-schema.json
slug: amazon-robomaker-openapi-create-deployment-job-response
source_filename: amazon-robomaker-openapi-create-deployment-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-deployment-job-response-schema.json\",\n  \"title\": \"CreateDeploymentJobResponse\",\n  \"description\": \"AWS RoboMaker is unable to process this request as the support for the AWS RoboMaker application deployment feature has ended. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/fleets.html.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the deployment job.\"\n        }\n      ]\n    },\n    \"fleet\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The target fleet\
  \ for the deployment job.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of the deployment job.\"\n        }\n      ]\n    },\n    \"deploymentApplicationConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentApplicationConfigs\"\n        },\n        {\n          \"description\": \"The deployment application configuration.\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The failure reason of the deployment job if it failed.\"\n        }\n      ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentJobErrorCode\"\n        },\n        {\n          \"description\": \"<p>The failure\
  \ code of the simulation job if it failed:</p> <dl> <dt>BadPermissionError</dt> <dd> <p>AWS Greengrass requires a service-level role permission to access other services. The role must include the <a href=\\\"https://console.aws.amazon.com/iam/home?#/policies/arn:aws:iam::aws:policy/service-role/AWSGreengrassResourceAccessRolePolicy$jsonEditor\\\"> <code>AWSGreengrassResourceAccessRolePolicy</code> managed policy</a>. </p> </dd> <dt>ExtractingBundleFailure</dt> <dd> <p>The robot application could not be extracted from the bundle.</p> </dd> <dt>FailureThresholdBreached</dt> <dd> <p>The percentage of robots that could not be updated exceeded the percentage set for the deployment.</p> </dd> <dt>GreengrassDeploymentFailed</dt> <dd> <p>The robot application could not be deployed to the robot.</p> </dd> <dt>GreengrassGroupVersionDoesNotExist</dt> <dd> <p>The AWS Greengrass group or version associated with a robot is missing.</p> </dd> <dt>InternalServerError</dt> <dd> <p>An internal error has\
  \ occurred. Retry your request, but if the problem persists, contact us with details.</p> </dd> <dt>MissingRobotApplicationArchitecture</dt> <dd> <p>The robot application does not have a source that matches the architecture of the robot.</p> </dd> <dt>MissingRobotDeploymentResource</dt> <dd> <p>One or more of the resources specified for the robot application are missing. For example, does the robot application have the correct launch package and launch file?</p> </dd> <dt>PostLaunchFileFailure</dt> <dd> <p>The post-launch script failed.</p> </dd> <dt>PreLaunchFileFailure</dt> <dd> <p>The pre-launch script failed.</p> </dd> <dt>ResourceNotFound</dt> <dd> <p>One or more deployment resources are missing. For example, do robot application source bundles still exist? </p> </dd> <dt>RobotDeploymentNoResponse</dt> <dd> <p>There is no response from the robot. It might not be powered on or connected to the internet.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/CreatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the fleet was created.\"\n        }\n      ]\n    },\n    \"deploymentConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentConfig\"\n        },\n        {\n          \"description\": \"The deployment configuration.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of all tags added to the deployment job.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-create-deployment-job-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: CreateDeploymentJobResponse
---
