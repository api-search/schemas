---
description: StartLoaderJobInput schema from Neptune
layout: schema
name: StartLoaderJobInput
properties_list:
- description: Amazon S3 URI identifying files or folders to load (s3://bucket/key).
  name: source
  type: string
- description: The data format of the files to load.
  name: format
  type: string
- description: The ARN of the IAM role with S3 access.
  name: iamRoleArn
  type: string
- description: The AWS Region of the S3 bucket.
  name: region
  type: string
- description: The load mode.
  name: mode
  type: string
- description: Whether to stop the load job on error.
  name: failOnError
  type: string
- description: The degree of parallelism for loading.
  name: parallelism
  type: string
- description: Optional parser configuration settings.
  name: parserConfiguration
  type: object
- description: Whether to update existing single-cardinality properties.
  name: updateSingleCardinalityProperties
  type: string
- description: Whether to queue the request if a load is already running.
  name: queueRequest
  type: string
- description: Load job IDs that must complete before this job runs.
  name: dependencies
  type: array
- description: For openCypher format, whether edge IDs are provided.
  name: userProvidedEdgeIds
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/data-start-loader-job-input-schema.json
slug: data-start-loader-job-input
source_filename: data-start-loader-job-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-loader-job-input-schema.json\",\n  \"title\": \"StartLoaderJobInput\",\n  \"description\": \"StartLoaderJobInput schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Amazon S3 URI identifying files or folders to load (s3://bucket/key).\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The data format of the files to load.\",\n      \"enum\": [\n        \"csv\",\n        \"opencypher\",\n        \"ntriples\",\n        \"nquads\",\n        \"rdfxml\",\n        \"turtle\"\n      ]\n    },\n    \"iamRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role with S3 access.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The AWS Region of the S3 bucket.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The load mode.\",\n      \"enum\": [\n        \"NEW\",\n        \"RESUME\",\n        \"AUTO\"\n      ],\n      \"default\": \"AUTO\"\n    },\n    \"failOnError\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to stop the load job on error.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"TRUE\"\n    },\n    \"parallelism\": {\n      \"type\": \"string\",\n      \"description\": \"The degree of parallelism for loading.\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"OVERSUBSCRIBE\"\n      ],\n      \"default\": \"HIGH\"\n    },\n    \"parserConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Optional parser configuration settings.\",\n      \"properties\": {\n        \"baseUri\": {\n          \"type\": \"string\"\n        },\n        \"namedGraphUri\"\
  : {\n          \"type\": \"string\"\n        },\n        \"allowEmptyStrings\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"updateSingleCardinalityProperties\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to update existing single-cardinality properties.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"FALSE\"\n    },\n    \"queueRequest\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to queue the request if a load is already running.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"FALSE\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"Load job IDs that must complete before this job runs.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"userProvidedEdgeIds\": {\n      \"type\": \"string\",\n      \"description\": \"For openCypher format, whether edge IDs are provided.\"\
  ,\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ]\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"format\",\n    \"iamRoleArn\",\n    \"region\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/data-start-loader-job-input-schema.json
tags:
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: StartLoaderJobInput
---
