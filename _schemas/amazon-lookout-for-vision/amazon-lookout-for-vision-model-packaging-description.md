---
description: Information about a model packaging job. For more information, see <a>DescribeModelPackagingJob</a>.
layout: schema
name: ModelPackagingDescription
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: ProjectName
  type: object
- description: ''
  name: ModelVersion
  type: object
- description: ''
  name: ModelPackagingConfiguration
  type: object
- description: ''
  name: ModelPackagingJobDescription
  type: object
- description: ''
  name: ModelPackagingMethod
  type: object
- description: ''
  name: ModelPackagingOutputDetails
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
- description: ''
  name: CreationTimestamp
  type: object
- description: ''
  name: LastUpdatedTimestamp
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-model-packaging-description-schema.json
slug: amazon-lookout-for-vision-model-packaging-description
source_filename: amazon-lookout-for-vision-model-packaging-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-packaging-description-schema.json\",\n  \"title\": \"ModelPackagingDescription\",\n  \"description\": \" Information about a model packaging job. For more information, see <a>DescribeModelPackagingJob</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingJobName\"\n        },\n        {\n          \"description\": \" The name of the model packaging job. \"\n        }\n      ]\n    },\n    \"ProjectName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProjectName\"\n        },\n        {\n          \"description\": \"The name of the project that's associated with a model that's in the model package. \"\n        }\n      ]\n\
  \    },\n    \"ModelVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelVersion\"\n        },\n        {\n          \"description\": \"The version of the model used in the model packaging job. \"\n        }\n      ]\n    },\n    \"ModelPackagingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingConfiguration\"\n        },\n        {\n          \"description\": \" The configuration information used in the model packaging job. \"\n        }\n      ]\n    },\n    \"ModelPackagingJobDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingJobDescription\"\n        },\n        {\n          \"description\": \"The description for the model packaging job. \"\n        }\n      ]\n    },\n    \"ModelPackagingMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingMethod\"\n        },\n        {\n          \"\
  description\": \"The AWS service used to package the job. Currently Lookout for Vision can package jobs with AWS IoT Greengrass. \"\n        }\n      ]\n    },\n    \"ModelPackagingOutputDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingOutputDetails\"\n        },\n        {\n          \"description\": \"Information about the output of the model packaging job. For more information, see <a>DescribeModelPackagingJob</a>. \"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingJobStatus\"\n        },\n        {\n          \"description\": \" The status of the model packaging job. \"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ModelPackagingStatusMessage\"\n        },\n        {\n          \"description\": \" The status message for the model packaging job. \"\n        }\n \
  \     ]\n    },\n    \"CreationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \" The Unix timestamp for the time and date that the model packaging job was created. \"\n        }\n      ]\n    },\n    \"LastUpdatedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \" The Unix timestamp for the time and date that the model packaging job was last updated. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-model-packaging-description-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: ModelPackagingDescription
---
