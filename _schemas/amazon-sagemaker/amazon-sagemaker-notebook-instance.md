---
description: NotebookInstance schema from Amazon SageMaker API
layout: schema
name: NotebookInstance
properties_list:
- description: The Amazon Resource Name (ARN) of the notebook instance.
  name: NotebookInstanceArn
  type: string
- description: The name of the notebook instance.
  name: NotebookInstanceName
  type: string
- description: The status of the notebook instance.
  name: NotebookInstanceStatus
  type: string
- description: The type of ML compute instance running the notebook.
  name: InstanceType
  type: string
- description: The ARN of the IAM role associated with the instance.
  name: RoleArn
  type: string
- description: The ID of the VPC subnet.
  name: SubnetId
  type: string
- description: The security groups associated with the instance.
  name: SecurityGroups
  type: array
- description: The URL that you use to connect to the Jupyter notebook.
  name: Url
  type: string
- description: The size of the ML storage volume in GB.
  name: VolumeSizeInGB
  type: integer
- description: A timestamp indicating when the notebook instance was created.
  name: CreationTime
  type: string
- description: A timestamp indicating when the notebook instance was last modified.
  name: LastModifiedTime
  type: string
provider_name: Amazon SageMaker
provider_slug: amazon-sagemaker
schema_file: json-schema/amazon-sagemaker-notebook-instance-schema.json
slug: amazon-sagemaker-notebook-instance
source_filename: amazon-sagemaker-notebook-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-notebook-instance-schema.json\",\n  \"title\": \"NotebookInstance\",\n  \"description\": \"NotebookInstance schema from Amazon SageMaker API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NotebookInstanceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the notebook instance.\"\n    },\n    \"NotebookInstanceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the notebook instance.\"\n    },\n    \"NotebookInstanceStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the notebook instance.\",\n      \"enum\": [\n        \"Pending\",\n        \"InService\",\n        \"Stopping\",\n        \"Stopped\",\n        \"Failed\",\n        \"Deleting\",\n        \"Updating\"\n      ]\n \
  \   },\n    \"InstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of ML compute instance running the notebook.\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role associated with the instance.\"\n    },\n    \"SubnetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC subnet.\"\n    },\n    \"SecurityGroups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The security groups associated with the instance.\"\n    },\n    \"Url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL that you use to connect to the Jupyter notebook.\"\n    },\n    \"VolumeSizeInGB\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the ML storage volume in GB.\"\n    },\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp\
  \ indicating when the notebook instance was created.\"\n    },\n    \"LastModifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp indicating when the notebook instance was last modified.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sagemaker/refs/heads/main/json-schema/amazon-sagemaker-notebook-instance-schema.json
tags:
- AI
- Inference
- Machine Learning
- MLOps
- Training
title: NotebookInstance
---
