---
description: DescribeSimulationJobResponse schema from openapi
layout: schema
name: DescribeSimulationJobResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: lastStartedAt
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: failureBehavior
  type: object
- description: ''
  name: failureCode
  type: object
- description: ''
  name: failureReason
  type: object
- description: ''
  name: clientRequestToken
  type: object
- description: ''
  name: outputLocation
  type: object
- description: ''
  name: loggingConfig
  type: object
- description: ''
  name: maxJobDurationInSeconds
  type: object
- description: ''
  name: simulationTimeMillis
  type: object
- description: ''
  name: iamRole
  type: object
- description: ''
  name: robotApplications
  type: object
- description: ''
  name: simulationApplications
  type: object
- description: ''
  name: dataSources
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: vpcConfig
  type: object
- description: ''
  name: networkInterface
  type: object
- description: ''
  name: compute
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-simulation-job-response-schema.json
slug: amazon-robomaker-openapi-describe-simulation-job-response
source_filename: amazon-robomaker-openapi-describe-simulation-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-job-response-schema.json\",\n  \"title\": \"DescribeSimulationJobResponse\",\n  \"description\": \"DescribeSimulationJobResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the simulation job.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the simulation job.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationJobStatus\"\n   \
  \     },\n        {\n          \"description\": \"The status of the simulation job.\"\n        }\n      ]\n    },\n    \"lastStartedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastStartedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job was last started.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation job was last updated.\"\n        }\n      ]\n    },\n    \"failureBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureBehavior\"\n        },\n        {\n          \"description\": \"The failure behavior for the simulation job.\"\n        }\n      ]\n    },\n    \"failureCode\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/SimulationJobErrorCode\"\n        },\n        {\n          \"description\": \"<p>The failure code of the simulation job if it failed:</p> <dl> <dt>InternalServiceError</dt> <dd> <p>Internal service error.</p> </dd> <dt>RobotApplicationCrash</dt> <dd> <p>Robot application exited abnormally.</p> </dd> <dt>SimulationApplicationCrash</dt> <dd> <p> Simulation application exited abnormally.</p> </dd> <dt>BadPermissionsRobotApplication</dt> <dd> <p>Robot application bundle could not be downloaded.</p> </dd> <dt>BadPermissionsSimulationApplication</dt> <dd> <p>Simulation application bundle could not be downloaded.</p> </dd> <dt>BadPermissionsS3Output</dt> <dd> <p>Unable to publish outputs to customer-provided S3 bucket.</p> </dd> <dt>BadPermissionsCloudwatchLogs</dt> <dd> <p>Unable to publish logs to customer-provided CloudWatch Logs resource.</p> </dd> <dt>SubnetIpLimitExceeded</dt> <dd> <p>Subnet IP limit exceeded.</p> </dd> <dt>ENILimitExceeded</dt> <dd> <p>ENI\
  \ limit exceeded.</p> </dd> <dt>BadPermissionsUserCredentials</dt> <dd> <p>Unable to use the Role provided.</p> </dd> <dt>InvalidBundleRobotApplication</dt> <dd> <p>Robot bundle cannot be extracted (invalid format, bundling error, or other issue).</p> </dd> <dt>InvalidBundleSimulationApplication</dt> <dd> <p>Simulation bundle cannot be extracted (invalid format, bundling error, or other issue).</p> </dd> <dt>RobotApplicationVersionMismatchedEtag</dt> <dd> <p>Etag for RobotApplication does not match value during version creation.</p> </dd> <dt>SimulationApplicationVersionMismatchedEtag</dt> <dd> <p>Etag for SimulationApplication does not match value during version creation.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"failureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"Details about why the simulation job failed. For more information about troubleshooting, see <a href=\\\
  \"https://docs.aws.amazon.com/robomaker/latest/dg/troubleshooting.html\\\">Troubleshooting</a>.\"\n        }\n      ]\n    },\n    \"clientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Unique, case-sensitive identifier that you provide to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"outputLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputLocation\"\n        },\n        {\n          \"description\": \"Location for output files generated by the simulation job.\"\n        }\n      ]\n    },\n    \"loggingConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfig\"\n        },\n        {\n          \"description\": \"The logging configuration.\"\n        }\n      ]\n    },\n    \"maxJobDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/JobDuration\"\n        },\n        {\n          \"description\": \"The maximum job duration in seconds. The value must be 8 days (691,200 seconds) or less.\"\n        }\n      ]\n    },\n    \"simulationTimeMillis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationTimeMillis\"\n        },\n        {\n          \"description\": \"The simulation job execution duration in milliseconds.\"\n        }\n      ]\n    },\n    \"iamRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRole\"\n        },\n        {\n          \"description\": \"The IAM role that allows the simulation instance to call the AWS APIs that are specified in its associated policies on your behalf.\"\n        }\n      ]\n    },\n    \"robotApplications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotApplicationConfigs\"\n        },\n        {\n          \"description\": \"A list of robot\
  \ applications.\"\n        }\n      ]\n    },\n    \"simulationApplications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationApplicationConfigs\"\n        },\n        {\n          \"description\": \"A list of simulation applications.\"\n        }\n      ]\n    },\n    \"dataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSources\"\n        },\n        {\n          \"description\": \"The data sources for the simulation job.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of all tags added to the specified simulation job.\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCConfigResponse\"\n        },\n        {\n          \"description\": \"The VPC configuration.\"\n        }\n      ]\n\
  \    },\n    \"networkInterface\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterface\"\n        },\n        {\n          \"description\": \"The network interface information for the simulation job.\"\n        }\n      ]\n    },\n    \"compute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeResponse\"\n        },\n        {\n          \"description\": \"Compute information for the simulation job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-job-response-schema.json
tags:
- Robotics
- Simulation
title: DescribeSimulationJobResponse
---
