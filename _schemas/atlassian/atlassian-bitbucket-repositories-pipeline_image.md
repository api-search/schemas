---
description: The definition of a Docker image that can be used for a Bitbucket Pipelines step execution context.
layout: schema
name: pipeline_image
properties_list:
- description: The name of the image. If the image is hosted on DockerHub the short name can be used, otherwise the fully qualified name is required here.
  name: name
  type: string
- description: The username needed to authenticate with the Docker registry. Only required when using a private Docker image.
  name: username
  type: string
- description: The password needed to authenticate with the Docker registry. Only required when using a private Docker image.
  name: password
  type: string
- description: The email needed to authenticate with the Docker registry. Only required when using a private Docker image.
  name: email
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-bitbucket-repositories-pipeline_image-schema.json
slug: atlassian-bitbucket-repositories-pipeline_image
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"pipeline_image\",\n  \"type\": \"object\",\n  \"description\": \"The definition of a Docker image that can be used for a Bitbucket Pipelines step execution context.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the image. If the image is hosted on DockerHub the short name can be used, otherwise the fully qualified name is required here.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The username needed to authenticate with the Docker registry. Only required when using a private Docker image.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The password needed to authenticate with the Docker registry. Only required when using a private Docker image.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email needed to authenticate\
  \ with the Docker registry. Only required when using a private Docker image.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-bitbucket-repositories-pipeline_image-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: pipeline_image
---
