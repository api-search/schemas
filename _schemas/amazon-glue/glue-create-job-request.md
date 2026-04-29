---
description: CreateJobRequest schema from Amazon Glue API
layout: schema
name: CreateJobRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: LogUri
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: ExecutionProperty
  type: object
- description: ''
  name: Command
  type: object
- description: ''
  name: DefaultArguments
  type: object
- description: ''
  name: NonOverridableArguments
  type: object
- description: ''
  name: Connections
  type: object
- description: ''
  name: MaxRetries
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
  name: Tags
  type: object
- description: ''
  name: NotificationProperty
  type: object
- description: ''
  name: GlueVersion
  type: object
- description: ''
  name: NumberOfWorkers
  type: object
- description: ''
  name: WorkerType
  type: object
- description: ''
  name: CodeGenConfigurationNodes
  type: object
- description: ''
  name: ExecutionClass
  type: object
- description: ''
  name: SourceControlDetails
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-job-request-schema.json
slug: glue-create-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-job-request-schema.json\",\n  \"title\": \"CreateJobRequest\",\n  \"description\": \"CreateJobRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name you assign to this job definition. It must be unique in your account.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"Description of the job being defined.\"\n        }\n      ]\n    },\n    \"LogUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UriString\"\n        },\n\
  \        {\n          \"description\": \"This field is reserved for future use.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleString\"\n        },\n        {\n          \"description\": \"The name or Amazon Resource Name (ARN) of the IAM role associated with this job.\"\n        }\n      ]\n    },\n    \"ExecutionProperty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionProperty\"\n        },\n        {\n          \"description\": \"An <code>ExecutionProperty</code> specifying the maximum number of concurrent runs allowed for this job.\"\n        }\n      ]\n    },\n    \"Command\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobCommand\"\n        },\n        {\n          \"description\": \"The <code>JobCommand</code> that runs this job.\"\n        }\n      ]\n    },\n    \"DefaultArguments\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/GenericMap\"\n        },\n        {\n          \"description\": \"<p>The default arguments for this job.</p> <p>You can specify arguments here that your own job-execution script consumes, as well as arguments that Glue itself consumes.</p> <p>Job arguments may be logged. Do not pass plaintext secrets as arguments. Retrieve secrets from a Glue Connection, Secrets Manager or other secret management mechanism if you intend to keep them within the Job. </p> <p>For information about how to specify and consume your own Job arguments, see the <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-python-calling.html\\\">Calling Glue APIs in Python</a> topic in the developer guide.</p> <p>For information about the key-value pairs that Glue consumes to set up your job, see the <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-glue-arguments.html\\\">Special Parameters Used by Glue</a> topic in the developer\
  \ guide.</p>\"\n        }\n      ]\n    },\n    \"NonOverridableArguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericMap\"\n        },\n        {\n          \"description\": \"Non-overridable arguments for this job, specified as name-value pairs.\"\n        }\n      ]\n    },\n    \"Connections\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectionsList\"\n        },\n        {\n          \"description\": \"The connections used for this job.\"\n        }\n      ]\n    },\n    \"MaxRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxRetries\"\n        },\n        {\n          \"description\": \"The maximum number of times to retry this job if it fails.\"\n        }\n      ]\n    },\n    \"AllocatedCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerValue\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\"\
  : \"<p>This parameter is deprecated. Use <code>MaxCapacity</code> instead.</p> <p>The number of Glue data processing units (DPUs) to allocate to this Job. You can allocate a minimum of 2 DPUs; the default is 10. A DPU is a relative measure of processing power that consists of 4 vCPUs of compute capacity and 16 GB of memory. For more information, see the <a href=\\\"https://aws.amazon.com/glue/pricing/\\\">Glue pricing page</a>.</p>This property is deprecated, use MaxCapacity instead.\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The job timeout in minutes. This is the maximum time that a job run can consume resources before it is terminated and enters <code>TIMEOUT</code> status. The default is 2,880 minutes (48 hours).\"\n        }\n      ]\n    },\n    \"MaxCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\
  \n        },\n        {\n          \"description\": \"<p>For Glue version 1.0 or earlier jobs, using the standard worker type, the number of Glue data processing units (DPUs) that can be allocated when this job runs. A DPU is a relative measure of processing power that consists of 4 vCPUs of compute capacity and 16 GB of memory. For more information, see the <a href=\\\"https://aws.amazon.com/glue/pricing/\\\">Glue pricing page</a>.</p> <p>Do not set <code>Max Capacity</code> if using <code>WorkerType</code> and <code>NumberOfWorkers</code>.</p> <p>The value that can be allocated for <code>MaxCapacity</code> depends on whether you are running a Python shell job or an Apache Spark ETL job:</p> <ul> <li> <p>When you specify a Python shell job (<code>JobCommand.Name</code>=\\\"pythonshell\\\"), you can allocate either 0.0625 or 1 DPU. The default is 0.0625 DPU.</p> </li> <li> <p>When you specify an Apache Spark ETL job (<code>JobCommand.Name</code>=\\\"glueetl\\\") or Apache Spark streaming\
  \ ETL job (<code>JobCommand.Name</code>=\\\"gluestreaming\\\"), you can allocate a minimum of 2 DPUs. The default is 10 DPUs. This job type cannot have a fractional DPU allocation.</p> </li> </ul> <p>For Glue version 2.0 jobs, you cannot instead specify a <code>Maximum capacity</code>. Instead, you should specify a <code>Worker type</code> and the <code>Number of workers</code>.</p>\"\n        }\n      ]\n    },\n    \"SecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the <code>SecurityConfiguration</code> structure to be used with this job.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags to use with this job. You may use tags to limit access to the job. For more information about tags in Glue, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-tags.html\\\
  \">Amazon Web Services Tags in Glue</a> in the developer guide.\"\n        }\n      ]\n    },\n    \"NotificationProperty\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationProperty\"\n        },\n        {\n          \"description\": \"Specifies configuration properties of a job notification.\"\n        }\n      ]\n    },\n    \"GlueVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueVersionString\"\n        },\n        {\n          \"description\": \"<p>Glue version determines the versions of Apache Spark and Python that Glue supports. The Python version indicates the version supported for jobs of type Spark. </p> <p>For more information about the available Glue versions and corresponding Spark and Python versions, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/add-job.html\\\">Glue version</a> in the developer guide.</p> <p>Jobs that are created without specifying a Glue version default to Glue\
  \ 0.9.</p>\"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of workers of a defined <code>workerType</code> that are allocated when a job runs.\"\n        }\n      ]\n    },\n    \"WorkerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkerType\"\n        },\n        {\n          \"description\": \"<p>The type of predefined worker that is allocated when a job runs. Accepts a value of Standard, G.1X, G.2X, or G.025X.</p> <ul> <li> <p>For the <code>Standard</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 50GB disk, and 2 executors per worker.</p> </li> <li> <p>For the <code>G.1X</code> worker type, each worker maps to 1 DPU (4 vCPU, 16 GB of memory, 64 GB disk), and provides 1 executor per worker. We recommend this worker type for memory-intensive jobs.</p> </li> <li>\
  \ <p>For the <code>G.2X</code> worker type, each worker maps to 2 DPU (8 vCPU, 32 GB of memory, 128 GB disk), and provides 1 executor per worker. We recommend this worker type for memory-intensive jobs.</p> </li> <li> <p>For the <code>G.025X</code> worker type, each worker maps to 0.25 DPU (2 vCPU, 4 GB of memory, 64 GB disk), and provides 1 executor per worker. We recommend this worker type for low volume streaming jobs. This worker type is only available for Glue version 3.0 streaming jobs.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"CodeGenConfigurationNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeGenConfigurationNodes\"\n        },\n        {\n          \"description\": \"The representation of a directed acyclic graph on which both the Glue Studio visual component and Glue Studio code generation is based.\"\n        }\n      ]\n    },\n    \"ExecutionClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionClass\"\
  \n        },\n        {\n          \"description\": \"<p>Indicates whether the job is run with a standard or flexible execution class. The standard execution-class is ideal for time-sensitive workloads that require fast job startup and dedicated resources.</p> <p>The flexible execution class is appropriate for time-insensitive jobs whose start and completion times may vary. </p> <p>Only jobs with Glue version 3.0 and above and command type <code>glueetl</code> will be allowed to set <code>ExecutionClass</code> to <code>FLEX</code>. The flexible execution class is available for Spark jobs.</p>\"\n        }\n      ]\n    },\n    \"SourceControlDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceControlDetails\"\n        },\n        {\n          \"description\": \"The details for a source control configuration for a job, allowing synchronization of job artifacts to or from a remote repository.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"Name\",\n    \"Role\",\n    \"Command\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-job-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateJobRequest
---
