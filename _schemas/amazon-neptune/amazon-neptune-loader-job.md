---
description: Represents a Neptune bulk loader job configuration and its status. The loader ingests data from Amazon S3 into a Neptune DB instance, supporting CSV for property graphs and N-Triples, N-Quads, RDF/XML, and Turtle for RDF data.
layout: schema
name: Amazon Neptune Loader Job
properties_list:
- description: 'Amazon S3 URI identifying the data file(s), folder, or multiple folders to load. Supported URI formats: s3://bucket/key, https://s3.amazonaws.com/bucket/key.'
  name: source
  type: string
- description: The data format of the source files to be loaded.
  name: format
  type: string
- description: The ARN of the IAM role that provides Neptune access to the S3 bucket. Can be a comma-separated list of role ARNs for cross-account access.
  name: iamRoleArn
  type: string
- description: The AWS Region of the S3 bucket containing the data to load.
  name: region
  type: string
- description: The load mode. NEW fails if data was previously loaded. RESUME continues a failed load from where it left off. AUTO resumes if possible, otherwise starts new.
  name: mode
  type: string
- description: Whether to stop the entire load job when an error is encountered.
  name: failOnError
  type: string
- description: The degree of parallelism for loading. LOW uses a single thread, MEDIUM uses num_vCPU/2, HIGH uses num_vCPU, OVERSUBSCRIBE uses all available resources.
  name: parallelism
  type: string
- description: Optional parser configuration settings for RDF data.
  name: parserConfiguration
  type: object
- description: Whether to update existing single-cardinality vertex properties with new values. Not supported for openCypher format.
  name: updateSingleCardinalityProperties
  type: string
- description: Whether to queue the request if a load job is already running. Neptune queues up to 64 jobs in FIFO order.
  name: queueRequest
  type: string
- description: An array of load job IDs that must complete successfully before this job runs.
  name: dependencies
  type: array
- description: For openCypher format only. TRUE means edge files contain an :ID column. FALSE means Neptune auto-generates edge IDs.
  name: userProvidedEdgeIds
  type: string
provider_name: Amazon Neptune
provider_slug: amazon-neptune
schema_file: json-schema/amazon-neptune-loader-job-schema.json
slug: amazon-neptune-loader-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/amazon-neptune/json-schema/amazon-neptune-loader-job-schema.json\",\n  \"title\": \"Amazon Neptune Loader Job\",\n  \"description\": \"Represents a Neptune bulk loader job configuration and its status. The loader ingests data from Amazon S3 into a Neptune DB instance, supporting CSV for property graphs and N-Triples, N-Quads, RDF/XML, and Turtle for RDF data.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"source\",\n    \"format\",\n    \"iamRoleArn\",\n    \"region\"\n  ],\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Amazon S3 URI identifying the data file(s), folder, or multiple folders to load. Supported URI formats: s3://bucket/key, https://s3.amazonaws.com/bucket/key.\",\n      \"examples\": [\n        \"s3://my-bucket/graph-data/\",\n        \"s3://my-bucket/data/vertices.csv\"\n      ]\n    },\n    \"\
  format\": {\n      \"type\": \"string\",\n      \"description\": \"The data format of the source files to be loaded.\",\n      \"enum\": [\n        \"csv\",\n        \"opencypher\",\n        \"ntriples\",\n        \"nquads\",\n        \"rdfxml\",\n        \"turtle\"\n      ]\n    },\n    \"iamRoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the IAM role that provides Neptune access to the S3 bucket. Can be a comma-separated list of role ARNs for cross-account access.\",\n      \"pattern\": \"^arn:aws[a-z-]*:iam::[0-9]+:role/\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The AWS Region of the S3 bucket containing the data to load.\",\n      \"examples\": [\n        \"us-east-1\",\n        \"eu-west-1\"\n      ]\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The load mode. NEW fails if data was previously loaded. RESUME continues a failed load from where it left off. AUTO resumes if possible,\
  \ otherwise starts new.\",\n      \"enum\": [\n        \"NEW\",\n        \"RESUME\",\n        \"AUTO\"\n      ],\n      \"default\": \"AUTO\"\n    },\n    \"failOnError\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to stop the entire load job when an error is encountered.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"TRUE\"\n    },\n    \"parallelism\": {\n      \"type\": \"string\",\n      \"description\": \"The degree of parallelism for loading. LOW uses a single thread, MEDIUM uses num_vCPU/2, HIGH uses num_vCPU, OVERSUBSCRIBE uses all available resources.\",\n      \"enum\": [\n        \"LOW\",\n        \"MEDIUM\",\n        \"HIGH\",\n        \"OVERSUBSCRIBE\"\n      ],\n      \"default\": \"HIGH\"\n    },\n    \"parserConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"Optional parser configuration settings for RDF data.\",\n      \"properties\": {\n        \"baseUri\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"The base URI for resolving relative URIs in the data.\"\n        },\n        \"namedGraphUri\": {\n          \"type\": \"string\",\n          \"description\": \"The default named graph URI for loaded triples.\"\n        },\n        \"allowEmptyStrings\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to allow empty string values for properties.\"\n        }\n      }\n    },\n    \"updateSingleCardinalityProperties\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to update existing single-cardinality vertex properties with new values. Not supported for openCypher format.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ],\n      \"default\": \"FALSE\"\n    },\n    \"queueRequest\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to queue the request if a load job is already running. Neptune queues up to 64 jobs in FIFO order.\",\n      \"enum\": [\n        \"TRUE\"\
  ,\n        \"FALSE\"\n      ],\n      \"default\": \"FALSE\"\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"An array of load job IDs that must complete successfully before this job runs.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"userProvidedEdgeIds\": {\n      \"type\": \"string\",\n      \"description\": \"For openCypher format only. TRUE means edge files contain an :ID column. FALSE means Neptune auto-generates edge IDs.\",\n      \"enum\": [\n        \"TRUE\",\n        \"FALSE\"\n      ]\n    }\n  },\n  \"$defs\": {\n    \"LoaderJobStatus\": {\n      \"type\": \"object\",\n      \"title\": \"Loader Job Status\",\n      \"description\": \"The status of a Neptune bulk loader job.\",\n      \"properties\": {\n        \"loadId\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for the load job.\"\n        },\n        \"overallStatus\": {\n          \"type\": \"object\",\n  \
  \        \"properties\": {\n            \"fullUri\": {\n              \"type\": \"string\",\n              \"description\": \"The S3 URI of the data source.\"\n            },\n            \"runNumber\": {\n              \"type\": \"integer\",\n              \"description\": \"The run number for this load.\"\n            },\n            \"retryNumber\": {\n              \"type\": \"integer\",\n              \"description\": \"The number of retries.\"\n            },\n            \"status\": {\n              \"type\": \"string\",\n              \"description\": \"The current status of the load job.\",\n              \"enum\": [\n                \"LOAD_NOT_STARTED\",\n                \"LOAD_IN_PROGRESS\",\n                \"LOAD_COMPLETED\",\n                \"LOAD_CANCELLED_BY_USER\",\n                \"LOAD_CANCELLED_DUE_TO_ERRORS\",\n                \"LOAD_FAILED\",\n                \"LOAD_UNEXPECTED_ERROR\",\n                \"LOAD_DATA_DEADLOCK\",\n                \"LOAD_DATA_FAILED_DUE_TO_FEED_MODIFIED_OR_DELETED\"\
  ,\n                \"LOAD_S3_READ_ERROR\",\n                \"LOAD_S3_ACCESS_DENIED_ERROR\",\n                \"LOAD_COMMITTED_W_WRITE_CONFLICTS\"\n              ]\n            },\n            \"totalTimeSpent\": {\n              \"type\": \"integer\",\n              \"description\": \"Total time spent on the load in seconds.\"\n            },\n            \"startTime\": {\n              \"type\": \"integer\",\n              \"description\": \"The start time as a Unix timestamp.\"\n            },\n            \"totalRecords\": {\n              \"type\": \"integer\",\n              \"description\": \"Total number of records processed.\"\n            },\n            \"totalDuplicates\": {\n              \"type\": \"integer\",\n              \"description\": \"Total number of duplicate records encountered.\"\n            },\n            \"parsingErrors\": {\n              \"type\": \"integer\",\n              \"description\": \"Total number of parsing errors.\"\n            },\n         \
  \   \"datatypeMismatchErrors\": {\n              \"type\": \"integer\",\n              \"description\": \"Total number of datatype mismatch errors.\"\n            },\n            \"insertErrors\": {\n              \"type\": \"integer\",\n              \"description\": \"Total number of insert errors.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-neptune/refs/heads/main/json-schema/amazon-neptune-loader-job-schema.json
tags:
- AWS
- Database
- Graph Database
- Gremlin
- Neptune
- Property Graph
- RDF
- SPARQL
title: Amazon Neptune Loader Job
---
