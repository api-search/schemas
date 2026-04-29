---
description: CreateDatasetRequest schema from Amazon Lookout for Vision API
layout: schema
name: CreateDatasetRequest
properties_list:
- description: ''
  name: DatasetType
  type: object
- description: ''
  name: DatasetSource
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-create-dataset-request-schema.json
slug: amazon-lookout-for-vision-create-dataset-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-dataset-request-schema.json\",\n  \"title\": \"CreateDatasetRequest\",\n  \"description\": \"CreateDatasetRequest schema from Amazon Lookout for Vision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetType\"\n        },\n        {\n          \"description\": \"The type of the dataset. Specify <code>train</code> for a training dataset. Specify <code>test</code> for a test dataset.\"\n        }\n      ]\n    },\n    \"DatasetSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatasetSource\"\n        },\n        {\n          \"description\": \"<p>The location of the manifest file that Amazon Lookout for Vision uses to create\
  \ the dataset.</p> <p>If you don't specify <code>DatasetSource</code>, an empty dataset is created and the operation synchronously returns. Later, you can add JSON Lines by calling <a>UpdateDatasetEntries</a>. </p> <p>If you specify a value for <code>DataSource</code>, the manifest at the S3 location is validated and used to create the dataset. The call to <code>CreateDataset</code> is asynchronous and might take a while to complete. To find out the current status, Check the value of <code>Status</code> returned in a call to <a>DescribeDataset</a>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatasetType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-create-dataset-request-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: CreateDatasetRequest
---
