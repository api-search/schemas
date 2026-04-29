---
description: DescribeSimulationOutput schema from Amazon SimSpace Weaver API
layout: schema
name: DescribeSimulationOutput
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: ExecutionId
  type: object
- description: ''
  name: LiveSimulationState
  type: object
- description: ''
  name: LoggingConfiguration
  type: object
- description: ''
  name: MaximumDuration
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SchemaError
  type: object
- description: ''
  name: SchemaS3Location
  type: object
- description: ''
  name: SnapshotS3Location
  type: object
- description: ''
  name: StartError
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: TargetStatus
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-describe-simulation-output-schema.json
slug: amazon-simspace-weaver-describe-simulation-output
source_filename: amazon-simspace-weaver-describe-simulation-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-describe-simulation-output-schema.json\",\n  \"title\": \"DescribeSimulationOutput\",\n  \"description\": \"DescribeSimulationOutput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the simulation. For more information about ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The time when the simulation was created, expressed as the number of seconds and milliseconds in UTC since the Unix epoch (0:0:0.000, January 1, 1970).\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the simulation.\"\n        }\n      ]\n    },\n    \"ExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"A universally unique identifier (UUID) for this simulation.\"\n        }\n      ]\n    },\n    \"LiveSimulationState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LiveSimulationState\"\n        },\n        {\n          \"description\": \"A collection of additional state information, such as domain and clock configuration.\"\n        }\n \
  \     ]\n    },\n    \"LoggingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfiguration\"\n        },\n        {\n          \"description\": \"Settings that control how SimSpace Weaver handles your simulation log data.\"\n        }\n      ]\n    },\n    \"MaximumDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeToLiveString\"\n        },\n        {\n          \"description\": \"The maximum running time of the simulation, specified as a number of minutes (m or M), hours (h or H), or days (d or D). The simulation stops when it reaches this limit. The maximum value is <code>14D</code>, or its equivalent in the other units. The default value is <code>14D</code>. A value equivalent to <code>0</code> makes the simulation immediately transition to <code>Stopping</code> as soon as it reaches <code>Started</code>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the simulation.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role that the simulation assumes to perform actions. For more information about ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>. For more information about IAM roles, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html\\\">IAM roles</a> in the <i>Identity and Access Management User Guide</i>.\"\n        }\n      ]\n    },\n    \"SchemaError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalString\"\
  \n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"An error message that SimSpace Weaver returns only if there is a problem with the simulation schema.SchemaError is no longer used, check StartError instead.\"\n        }\n      ]\n    },\n    \"SchemaS3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The location of the simulation schema in Amazon Simple Storage Service (Amazon S3). For more information about Amazon S3, see the <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html\\\"> <i>Amazon Simple Storage Service User Guide</i> </a>.\"\n        }\n      ]\n    },\n    \"SnapshotS3Location\": {\n      \"$ref\": \"#/components/schemas/S3Location\"\n    },\n    \"StartError\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalString\"\n        },\n        {\n          \"description\":\
  \ \"An error message that SimSpace Weaver returns only if a problem occurs when the simulation is in the <code>STARTING</code> state.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationStatus\"\n        },\n        {\n          \"description\": \"The current lifecycle state of the simulation.\"\n        }\n      ]\n    },\n    \"TargetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationTargetStatus\"\n        },\n        {\n          \"description\": \"The desired lifecycle state of the simulation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-describe-simulation-output-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: DescribeSimulationOutput
---
