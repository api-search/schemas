---
description: A quantum task submitted to an Amazon Braket device (QPU or simulator)
layout: schema
name: Quantum Task
properties_list:
- description: ARN of the quantum task
  name: quantumTaskArn
  type: string
- description: ARN of the quantum device the task is submitted to
  name: deviceArn
  type: string
- description: Number of times the circuit is executed
  name: shots
  type: integer
- description: S3 bucket for task result output
  name: outputS3Bucket
  type: string
- description: S3 key prefix for task result output
  name: outputS3KeyPrefix
  type: string
- description: Current status of the quantum task
  name: status
  type: string
- description: Reason for task failure if status is FAILED
  name: failureReason
  type: string
- description: Timestamp when the task was created
  name: createdAt
  type: string
- description: Timestamp when the task ended
  name: endedAt
  type: string
- description: Metadata tags for the quantum task
  name: tags
  type: object
provider_name: Amazon Braket
provider_slug: amazon-braket
schema_file: json-schema/braket-task-schema.json
slug: braket-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-braket/main/json-schema/braket-task-schema.json\",\n  \"title\": \"Quantum Task\",\n  \"description\": \"A quantum task submitted to an Amazon Braket device (QPU or simulator)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"quantumTaskArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the quantum task\",\n      \"pattern\": \"^arn:aws[a-z\\\\-]*:braket:[a-z0-9\\\\-]+:[0-9]{12}:quantum-task/[a-z0-9\\\\-]+$\"\n    },\n    \"deviceArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the quantum device the task is submitted to\"\n    },\n    \"shots\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times the circuit is executed\",\n      \"minimum\": 1\n    },\n    \"outputS3Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"S3 bucket for task result output\"\n\
  \    },\n    \"outputS3KeyPrefix\": {\n      \"type\": \"string\",\n      \"description\": \"S3 key prefix for task result output\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"CREATED\", \"QUEUED\", \"RUNNING\", \"COMPLETED\", \"FAILED\", \"CANCELLING\", \"CANCELLED\"],\n      \"description\": \"Current status of the quantum task\"\n    },\n    \"failureReason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for task failure if status is FAILED\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the task was created\"\n    },\n    \"endedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the task ended\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata tags for the quantum task\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n\
  \    }\n  },\n  \"required\": [\"quantumTaskArn\", \"deviceArn\", \"shots\", \"outputS3Bucket\", \"status\", \"createdAt\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-braket/refs/heads/main/json-schema/braket-task-schema.json
tags:
- Quantum Computing
- Quantum Hardware
- Hybrid Quantum-Classical
- QPU
- Quantum Simulation
- AWS
- Amazon Web Services
- Research
- HPC
title: Quantum Task
---
