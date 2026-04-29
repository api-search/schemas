---
description: Schema defining the structure of an AWS Batch job definition resource, including container properties, retry strategy, timeout, scheduling, and resource requirements.
layout: schema
name: AWS Batch Job Definition
properties_list:
- description: The name of the job definition.
  name: jobDefinitionName
  type: string
- description: The Amazon Resource Name (ARN) for the job definition.
  name: jobDefinitionArn
  type: string
- description: The revision of the job definition.
  name: revision
  type: integer
- description: The status of the job definition.
  name: status
  type: string
- description: The type of job definition.
  name: type
  type: string
- description: The scheduling priority of the job definition.
  name: schedulingPriority
  type: integer
- description: Default parameters or parameter substitution placeholders in the job definition.
  name: parameters
  type: object
- description: ''
  name: retryStrategy
  type: object
- description: ''
  name: containerProperties
  type: object
- description: ''
  name: nodeProperties
  type: object
- description: ''
  name: timeout
  type: object
- description: The tags that are applied to the job definition.
  name: tags
  type: object
- description: The platform capabilities required by the job definition.
  name: platformCapabilities
  type: array
- description: Whether to propagate tags from the job definition to the job.
  name: propagateTags
  type: boolean
provider_name: Amazon Batch
provider_slug: amazon-batch
schema_file: json-schema/amazon-batch-schema.json
slug: amazon-batch
source_filename: amazon-batch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-batch/job-definition\",\n  \"title\": \"AWS Batch Job Definition\",\n  \"description\": \"Schema defining the structure of an AWS Batch job definition resource, including container properties, retry strategy, timeout, scheduling, and resource requirements.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"jobDefinitionName\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"jobDefinitionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job definition.\"\n    },\n    \"jobDefinitionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the job definition.\"\n    },\n    \"revision\": {\n      \"type\": \"integer\",\n      \"description\": \"The revision of the job definition.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the job\
  \ definition.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"container\",\n        \"multinode\"\n      ],\n      \"description\": \"The type of job definition.\"\n    },\n    \"schedulingPriority\": {\n      \"type\": \"integer\",\n      \"description\": \"The scheduling priority of the job definition.\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Default parameters or parameter substitution placeholders in the job definition.\"\n    },\n    \"retryStrategy\": {\n      \"$ref\": \"#/$defs/RetryStrategy\"\n    },\n    \"containerProperties\": {\n      \"$ref\": \"#/$defs/ContainerProperties\"\n    },\n    \"nodeProperties\": {\n      \"$ref\": \"#/$defs/NodeProperties\"\n    },\n    \"timeout\": {\n      \"$ref\": \"#/$defs/JobTimeout\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n      \
  \  \"type\": \"string\"\n      },\n      \"description\": \"The tags that are applied to the job definition.\"\n    },\n    \"platformCapabilities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"EC2\",\n          \"FARGATE\"\n        ]\n      },\n      \"description\": \"The platform capabilities required by the job definition.\"\n    },\n    \"propagateTags\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to propagate tags from the job definition to the job.\"\n    }\n  },\n  \"$defs\": {\n    \"RetryStrategy\": {\n      \"type\": \"object\",\n      \"description\": \"The retry strategy for failed jobs.\",\n      \"properties\": {\n        \"attempts\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 10,\n          \"description\": \"The number of times to retry a failed job.\"\n        },\n        \"evaluateOnExit\": {\n          \"type\": \"array\",\n    \
  \      \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"onStatusReason\": {\n                \"type\": \"string\"\n              },\n              \"onReason\": {\n                \"type\": \"string\"\n              },\n              \"onExitCode\": {\n                \"type\": \"string\"\n              },\n              \"action\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"RETRY\",\n                  \"EXIT\"\n                ]\n              }\n            },\n            \"required\": [\n              \"action\"\n            ]\n          }\n        }\n      }\n    },\n    \"ContainerProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Container properties for a single-node job.\",\n      \"properties\": {\n        \"image\": {\n          \"type\": \"string\",\n          \"description\": \"The image used to start a container.\"\n        },\n        \"command\": {\n      \
  \    \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The command that is passed to the container.\"\n        },\n        \"jobRoleArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the IAM role for the container.\"\n        },\n        \"executionRoleArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the execution role for Fargate tasks.\"\n        },\n        \"environment\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"description\": \"The environment variables to pass to a container.\"\n        },\n        \"resourceRequirements\": {\n          \"type\": \"array\"\
  ,\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"value\",\n              \"type\"\n            ],\n            \"properties\": {\n              \"value\": {\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"GPU\",\n                  \"VCPU\",\n                  \"MEMORY\"\n                ]\n              }\n            }\n          },\n          \"description\": \"The type and amount of resources to assign to a container.\"\n        },\n        \"mountPoints\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"containerPath\": {\n                \"type\": \"string\"\n              },\n              \"readOnly\": {\n                \"type\": \"boolean\"\n              },\n              \"sourceVolume\": {\n            \
  \    \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"volumes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"host\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"sourcePath\": {\n                    \"type\": \"string\"\n                  }\n                }\n              },\n              \"efsVolumeConfiguration\": {\n                \"type\": \"object\"\n              }\n            }\n          }\n        },\n        \"logConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"logDriver\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"json-file\",\n                \"syslog\",\n                \"journald\",\n                \"gelf\",\n\
  \                \"fluentd\",\n                \"awslogs\",\n                \"splunk\"\n              ]\n            },\n            \"options\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n              }\n            },\n            \"secretOptions\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\"\n              }\n            }\n          }\n        },\n        \"privileged\": {\n          \"type\": \"boolean\"\n        },\n        \"readonlyRootFilesystem\": {\n          \"type\": \"boolean\"\n        },\n        \"user\": {\n          \"type\": \"string\"\n        },\n        \"linuxParameters\": {\n          \"type\": \"object\"\n        },\n        \"fargatePlatformConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"platformVersion\": {\n              \"type\": \"string\"\n            }\n          }\n \
  \       },\n        \"networkConfiguration\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"assignPublicIp\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"ENABLED\",\n                \"DISABLED\"\n              ]\n            }\n          }\n        }\n      }\n    },\n    \"NodeProperties\": {\n      \"type\": \"object\",\n      \"description\": \"An object that represents the node properties of a multi-node parallel job.\",\n      \"required\": [\n        \"numNodes\",\n        \"mainNode\",\n        \"nodeRangeProperties\"\n      ],\n      \"properties\": {\n        \"numNodes\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of nodes that are associated with a multi-node parallel job.\"\n        },\n        \"mainNode\": {\n          \"type\": \"integer\",\n          \"description\": \"The node index value for the main node of a multi-node parallel job.\"\n        },\n        \"nodeRangeProperties\"\
  : {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"targetNodes\": {\n                \"type\": \"string\"\n              },\n              \"container\": {\n                \"$ref\": \"#/$defs/ContainerProperties\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"JobTimeout\": {\n      \"type\": \"object\",\n      \"description\": \"Job timeout configuration.\",\n      \"properties\": {\n        \"attemptDurationSeconds\": {\n          \"type\": \"integer\",\n          \"minimum\": 60,\n          \"description\": \"The job timeout time, in seconds.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-batch/refs/heads/main/json-schema/amazon-batch-schema.json
tags:
- AWS
- Batch Computing
- Compute
- Containers
- HPC
- Job Scheduling
- Serverless
- Fargate
- EKS
- Spot Instances
title: AWS Batch Job Definition
---
