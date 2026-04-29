---
description: Information about a simulation job request.
layout: schema
name: SimulationJobRequest
properties_list:
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
  name: iamRole
  type: object
- description: ''
  name: failureBehavior
  type: object
- description: ''
  name: useDefaultApplications
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
  name: vpcConfig
  type: object
- description: ''
  name: compute
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-simulation-job-request-schema.json
slug: amazon-robomaker-openapi-simulation-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-job-request-schema.json\",\n  \"title\": \"SimulationJobRequest\",\n  \"description\": \"Information about a simulation job request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputLocation\": {\n      \"$ref\": \"#/components/schemas/OutputLocation\"\n    },\n    \"loggingConfig\": {\n      \"$ref\": \"#/components/schemas/LoggingConfig\"\n    },\n    \"maxJobDurationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDuration\"\n        },\n        {\n          \"description\": \"The maximum simulation job duration in seconds. The value must be 8 days (691,200 seconds) or less.\"\n        }\n      ]\n    },\n    \"iamRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRole\"\
  \n        },\n        {\n          \"description\": \"The IAM role name that allows the simulation instance to call the AWS APIs that are specified in its associated policies on your behalf. This is how credentials are passed in to your simulation job. \"\n        }\n      ]\n    },\n    \"failureBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureBehavior\"\n        },\n        {\n          \"description\": \"<p>The failure behavior the simulation job.</p> <dl> <dt>Continue</dt> <dd> <p>Leaves the host running for its maximum timeout duration after a <code>4XX</code> error code.</p> </dd> <dt>Fail</dt> <dd> <p>Stop the simulation job and terminate the instance.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"useDefaultApplications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoxedBoolean\"\n        },\n        {\n          \"description\": \"A Boolean indicating whether to use default applications in the\
  \ simulation job. Default applications include Gazebo, rqt, rviz and terminal access. \"\n        }\n      ]\n    },\n    \"robotApplications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotApplicationConfigs\"\n        },\n        {\n          \"description\": \"The robot applications to use in the simulation job.\"\n        }\n      ]\n    },\n    \"simulationApplications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationApplicationConfigs\"\n        },\n        {\n          \"description\": \"The simulation applications to use in the simulation job.\"\n        }\n      ]\n    },\n    \"dataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceConfigs\"\n        },\n        {\n          \"description\": \"<p>Specify data sources to mount read-only files from S3 into your simulation. These files are available under <code>/opt/robomaker/datasources/data_source_name</code>.\
  \ </p> <note> <p>There is a limit of 100 files and a combined size of 25GB for all <code>DataSourceConfig</code> objects. </p> </note>\"\n        }\n      ]\n    },\n    \"vpcConfig\": {\n      \"$ref\": \"#/components/schemas/VPCConfig\"\n    },\n    \"compute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compute\"\n        },\n        {\n          \"description\": \"Compute information for the simulation job\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A map that contains tag keys and tag values that are attached to the simulation job request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"maxJobDurationInSeconds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-job-request-schema.json
tags:
- AWS
- Robotics
- Simulation
title: SimulationJobRequest
---
