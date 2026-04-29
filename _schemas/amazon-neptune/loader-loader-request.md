---
description: LoaderRequest schema from Neptune
layout: schema
name: LoaderRequest
properties_list:
- description: 'Amazon S3 URI identifying the data file(s), folder, or multiple folders to load. Supported URI formats: s3://bucket_name/key, https://s3.amazonaws.com/bucket_name/key, https://s3.region.amazonaws.com/'
  name: source
  type: string
- description: The data format of the source files.
  name: format
  type: string
- description: The ARN of the IAM role that provides Neptune access to the S3 bucket. Can be a comma-separated list for cross-account access.
  name: iamRoleArn
  type: string
- description: The AWS Region of the S3 bucket. Must match the Neptune cluster region or be accessible cross-region.
  name: region
  type: string
- description: The load mode. NEW fails if data was previously loaded. RESUME continues a failed load. AUTO resumes or starts new as needed.
  name: mode
  type: string
- description: Whether to stop the entire load job on error.
  name: failOnError
  type: string
- description: The degree of parallelism for loading. LOW uses a single thread, MEDIUM uses num_vCPU/2, HIGH uses num_vCPU, OVERSUBSCRIBE uses all available resources.
  name: parallelism
  type: string
- description: Optional parser configuration settings for RDF data.
  name: parserConfiguration
  type: object
- description: Whether to update existing single-cardinality vertex properties. Not supported for openCypher format.
  name: updateSingleCardinalityProperties
  type: string
- description: Whether to queue the request if a load is already running. Neptune queues up to 64 jobs in FIFO order.
  name: queueRequest
  type: string
- description: Array of load job IDs that must complete successfully before this job runs.
  name: dependencies
  type: array
- description: For openCypher format only. TRUE requires an :ID column in edge files. FALSE auto-generates edge IDs.
  name: userProvidedEdgeIds
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/loader-loader-request-schema.json
slug: loader-loader-request
source_filename: loader-loader-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-request-schema.json\",\n  \"title\": \"LoaderRequest\",\n  \"description\": \"LoaderRequest schema from Neptune\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Amazon S3 URI identifying the data file(s), folder, or multiple folders to load. Supported URI formats: s3://bucket_name/key, https://s3.amazonaws.com/bucket_name/key, https://s3.region.amazonaws.com/bucket_name/key.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The data format of the source files.\",\n      \"enum\": [\n        \"csv\",\n        \"opencypher\",\n        \"ntriples\",\n        \"nquads\",\n        \"rdfxml\",\n        \"turtle\"\n      ]\n    },\n    \"iamRoleArn\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The ARN of the IAM role that provides Neptune access to the S3 bucket. Can be a comma-separated list for cross-account access.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS Region of the S3 bucket. Must match the Neptune cluster region or be accessible cross-region.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The load mode. NEW fails if data was previously loaded. RESUME continues a failed load. AUTO resumes or starts new as needed.\",\n      \"enum\": [\n        \"NEW\",\n        \"RESUME\",\n        \"AUTO\"\n      ],\n      \"default\": \"AUTO\"\n    },\n    \"failOnError\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to stop the entire load job on error.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"TRUE\"\n    },\n    \"parallelism\": {\n      \"type\": \"string\",\n      \"description\": \"The degree of parallelism\
  \ for loading. LOW uses a single thread, MEDIUM uses num_vCPU/2, HIGH uses num_vCPU, OVERSUBSCRIBE uses all available resources.\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"OVERSUBSCRIBE\"\n      ],\n      \"default\": \"HIGH\"\n    },\n    \"parserConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Optional parser configuration settings for RDF data.\",\n      \"properties\": {\n        \"baseUri\": {\n          \"type\": \"string\",\n          \"description\": \"The base URI for relative URIs in the data.\"\n        },\n        \"namedGraphUri\": {\n          \"type\": \"string\",\n          \"description\": \"The default named graph URI for loaded triples.\"\n        },\n        \"allowEmptyStrings\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to allow empty string property values.\"\n        }\n      }\n    },\n    \"updateSingleCardinalityProperties\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Whether to update existing single-cardinality vertex properties. Not supported for openCypher format.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"FALSE\"\n    },\n    \"queueRequest\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to queue the request if a load is already running. Neptune queues up to 64 jobs in FIFO order.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"FALSE\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"Array of load job IDs that must complete successfully before this job runs.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"userProvidedEdgeIds\": {\n      \"type\": \"string\",\n      \"description\": \"For openCypher format only. TRUE requires an :ID column in edge files. FALSE auto-generates edge IDs.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\
  \n      ]\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"format\",\n    \"iamRoleArn\",\n    \"region\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/loader-loader-request-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: LoaderRequest
---
