---
description: Schema for a Google Cloud AutoML model resource.
layout: schema
name: AutoML Model
properties_list:
- description: Resource name of the model.
  name: name
  type: string
- description: Human-readable display name for the model.
  name: displayName
  type: string
- description: ID of the dataset used to train the model.
  name: datasetId
  type: string
- description: Timestamp when the model was created.
  name: createTime
  type: string
- description: Timestamp when the model was last updated.
  name: updateTime
  type: string
- description: Deployment state of the model.
  name: deploymentState
  type: string
- description: Entity tag for optimistic concurrency control.
  name: etag
  type: string
provider_name: Google Cloud AutoML
provider_slug: google-cloud-automl
schema_file: json-schema/model.json
slug: model
source_filename: model.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-automl/refs/heads/main/json-schema/model.json\",\n  \"title\": \"AutoML Model\",\n  \"description\": \"Schema for a Google Cloud AutoML model resource.\",\n  \"type\": \"object\",\n  \"required\": [\"displayName\", \"datasetId\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the model.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the model.\"\n    },\n    \"datasetId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the dataset used to train the model.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the model was created.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"\
  format\": \"date-time\",\n      \"description\": \"Timestamp when the model was last updated.\"\n    },\n    \"deploymentState\": {\n      \"type\": \"string\",\n      \"enum\": [\"DEPLOYMENT_STATE_UNSPECIFIED\", \"DEPLOYED\", \"UNDEPLOYED\"],\n      \"description\": \"Deployment state of the model.\"\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"Entity tag for optimistic concurrency control.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-automl/refs/heads/main/json-schema/model.json
tags:
- AutoML
- Custom Models
- Google Cloud
- Machine Learning
- Training
title: AutoML Model
---
