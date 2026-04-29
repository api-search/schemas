---
description: Request to create a new session.
layout: schema
name: CreateSessionRequest
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: Command
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: IdleTimeout
  type: object
- description: ''
  name: DefaultArguments
  type: object
- description: ''
  name: Connections
  type: object
- description: ''
  name: MaxCapacity
  type: object
- description: ''
  name: NumberOfWorkers
  type: object
- description: ''
  name: WorkerType
  type: object
- description: ''
  name: SecurityConfiguration
  type: object
- description: ''
  name: GlueVersion
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: RequestOrigin
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-session-request-schema.json
slug: glue-create-session-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-session-request-schema.json\",\n  \"title\": \"CreateSessionRequest\",\n  \"description\": \"Request to create a new session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The ID of the session request. \"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"The description of the session. \"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationRoleArn\"\n        },\n        {\n          \"description\": \"The IAM Role\
  \ ARN \"\n        }\n      ]\n    },\n    \"Command\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SessionCommand\"\n        },\n        {\n          \"description\": \"The <code>SessionCommand</code> that runs the job. \"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \" The number of minutes before session times out. Default for Spark ETL jobs is 48 hours (2880 minutes), the maximum session lifetime for this job type. Consult the documentation for other job types. \"\n        }\n      ]\n    },\n    \"IdleTimeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \" The number of minutes when idle before session times out. Default for Spark ETL jobs is value of Timeout. Consult the documentation for other job types. \"\n       \
  \ }\n      ]\n    },\n    \"DefaultArguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationArgumentsMap\"\n        },\n        {\n          \"description\": \"A map array of key-value pairs. Max is 75 pairs. \"\n        }\n      ]\n    },\n    \"Connections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionsList\"\n        },\n        {\n          \"description\": \"The number of connections to use for the session. \"\n        }\n      ]\n    },\n    \"MaxCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"The number of Glue data processing units (DPUs) that can be allocated when the job runs. A DPU is a relative measure of processing power that consists of 4 vCPUs of compute capacity and 16 GB memory. \"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of workers of a defined <code>WorkerType</code> to use for the session. \"\n        }\n      ]\n    },\n    \"WorkerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkerType\"\n        },\n        {\n          \"description\": \"<p>The type of predefined worker that is allocated to use for the session. Accepts a value of Standard, G.1X, G.2X, or G.025X.</p> <ul> <li> <p>For the <code>Standard</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 50GB disk, and 2 executors per worker.</p> </li> <li> <p>For the <code>G.1X</code> worker type, each worker maps to 1 DPU (4 vCPU, 16 GB of memory, 64 GB disk), and provides 1 executor per worker. We recommend this worker type for memory-intensive jobs.</p> </li> <li> <p>For the <code>G.2X</code> worker type, each worker maps to 2 DPU (8 vCPU, 32 GB of memory, 128 GB disk),\
  \ and provides 1 executor per worker. We recommend this worker type for memory-intensive jobs.</p> </li> <li> <p>For the <code>G.025X</code> worker type, each worker maps to 0.25 DPU (2 vCPU, 4 GB of memory, 64 GB disk), and provides 1 executor per worker. We recommend this worker type for low volume streaming jobs. This worker type is only available for Glue version 3.0 streaming jobs.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"SecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the SecurityConfiguration structure to be used with the session \"\n        }\n      ]\n    },\n    \"GlueVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueVersionString\"\n        },\n        {\n          \"description\": \"The Glue version determines the versions of Apache Spark and Python that Glue supports. The GlueVersion must be\
  \ greater than 2.0. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The map of key value pairs (tags) belonging to the session.\"\n        }\n      ]\n    },\n    \"RequestOrigin\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrchestrationNameString\"\n        },\n        {\n          \"description\": \"The origin of the request. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\",\n    \"Role\",\n    \"Command\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-session-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateSessionRequest
---
