---
description: StartJobRunRequest schema from Amazon Glue API
layout: schema
name: StartJobRunRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobRunId
  type: object
- description: ''
  name: Arguments
  type: object
- description: ''
  name: AllocatedCapacity
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: MaxCapacity
  type: object
- description: ''
  name: SecurityConfiguration
  type: object
- description: ''
  name: NotificationProperty
  type: object
- description: ''
  name: WorkerType
  type: object
- description: ''
  name: NumberOfWorkers
  type: object
- description: ''
  name: ExecutionClass
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-start-job-run-request-schema.json
slug: glue-start-job-run-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-job-run-request-schema.json\",\n  \"title\": \"StartJobRunRequest\",\n  \"description\": \"StartJobRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the job definition to use.\"\n        }\n      ]\n    },\n    \"JobRunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The ID of a previous <code>JobRun</code> to retry.\"\n        }\n      ]\n    },\n    \"Arguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericMap\"\n        },\n        {\n          \"description\"\
  : \"<p>The job arguments specifically for this run. For this job run, they replace the default arguments set in the job definition itself.</p> <p>You can specify arguments here that your own job-execution script consumes, as well as arguments that Glue itself consumes.</p> <p>Job arguments may be logged. Do not pass plaintext secrets as arguments. Retrieve secrets from a Glue Connection, Secrets Manager or other secret management mechanism if you intend to keep them within the Job. </p> <p>For information about how to specify and consume your own Job arguments, see the <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-python-calling.html\\\">Calling Glue APIs in Python</a> topic in the developer guide.</p> <p>For information about the key-value pairs that Glue consumes to set up your job, see the <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-glue-arguments.html\\\">Special Parameters Used by Glue</a> topic in the developer guide.</p>\"\
  \n        }\n      ]\n    },\n    \"AllocatedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerValue\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"<p>This field is deprecated. Use <code>MaxCapacity</code> instead.</p> <p>The number of Glue data processing units (DPUs) to allocate to this JobRun. You can allocate a minimum of 2 DPUs; the default is 10. A DPU is a relative measure of processing power that consists of 4 vCPUs of compute capacity and 16 GB of memory. For more information, see the <a href=\\\"https://aws.amazon.com/glue/pricing/\\\">Glue pricing page</a>.</p>This property is deprecated, use MaxCapacity instead.\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"<p>The <code>JobRun</code> timeout in minutes. This is the maximum time that a job run can consume\
  \ resources before it is terminated and enters <code>TIMEOUT</code> status. This value overrides the timeout value set in the parent job.</p> <p>Streaming jobs do not have a timeout. The default for non-streaming jobs is 2,880 minutes (48 hours).</p>\"\n        }\n      ]\n    },\n    \"MaxCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"<p>The number of Glue data processing units (DPUs) that can be allocated when this job runs. A DPU is a relative measure of processing power that consists of 4 vCPUs of compute capacity and 16 GB of memory. For more information, see the <a href=\\\"https://aws.amazon.com/glue/pricing/\\\">Glue pricing page</a>.</p> <p>Do not set <code>Max Capacity</code> if using <code>WorkerType</code> and <code>NumberOfWorkers</code>.</p> <p>The value that can be allocated for <code>MaxCapacity</code> depends on whether you are running a Python shell job, or\
  \ an Apache Spark ETL job:</p> <ul> <li> <p>When you specify a Python shell job (<code>JobCommand.Name</code>=\\\"pythonshell\\\"), you can allocate either 0.0625 or 1 DPU. The default is 0.0625 DPU.</p> </li> <li> <p>When you specify an Apache Spark ETL job (<code>JobCommand.Name</code>=\\\"glueetl\\\"), you can allocate a minimum of 2 DPUs. The default is 10 DPUs. This job type cannot have a fractional DPU allocation.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"SecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the <code>SecurityConfiguration</code> structure to be used with this job run.\"\n        }\n      ]\n    },\n    \"NotificationProperty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationProperty\"\n        },\n        {\n          \"description\": \"Specifies configuration properties of a job run notification.\"\
  \n        }\n      ]\n    },\n    \"WorkerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkerType\"\n        },\n        {\n          \"description\": \"<p>The type of predefined worker that is allocated when a job runs. Accepts a value of Standard, G.1X, G.2X, or G.025X.</p> <ul> <li> <p>For the <code>Standard</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 50GB disk, and 2 executors per worker.</p> </li> <li> <p>For the <code>G.1X</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 64GB disk, and 1 executor per worker.</p> </li> <li> <p>For the <code>G.2X</code> worker type, each worker provides 8 vCPU, 32 GB of memory and a 128GB disk, and 1 executor per worker.</p> </li> <li> <p>For the <code>G.025X</code> worker type, each worker maps to 0.25 DPU (2 vCPU, 4 GB of memory, 64 GB disk), and provides 1 executor per worker. We recommend this worker type for low volume streaming jobs. This worker type is only\
  \ available for Glue version 3.0 streaming jobs.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of workers of a defined <code>workerType</code> that are allocated when a job runs.\"\n        }\n      ]\n    },\n    \"ExecutionClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionClass\"\n        },\n        {\n          \"description\": \"<p>Indicates whether the job is run with a standard or flexible execution class. The standard execution-class is ideal for time-sensitive workloads that require fast job startup and dedicated resources.</p> <p>The flexible execution class is appropriate for time-insensitive jobs whose start and completion times may vary. </p> <p>Only jobs with Glue version 3.0 and above and command type <code>glueetl</code> will be allowed to set\
  \ <code>ExecutionClass</code> to <code>FLEX</code>. The flexible execution class is available for Spark jobs.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-start-job-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: StartJobRunRequest
---
