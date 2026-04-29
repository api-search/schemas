---
description: CreateMLTransformRequest schema from Amazon Glue API
layout: schema
name: CreateMLTransformRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: InputRecordTables
  type: object
- description: ''
  name: Parameters
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: GlueVersion
  type: object
- description: ''
  name: MaxCapacity
  type: object
- description: ''
  name: WorkerType
  type: object
- description: ''
  name: NumberOfWorkers
  type: object
- description: ''
  name: Timeout
  type: object
- description: ''
  name: MaxRetries
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: TransformEncryption
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-ml-transform-request-schema.json
slug: glue-create-ml-transform-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-ml-transform-request-schema.json\",\n  \"title\": \"CreateMLTransformRequest\",\n  \"description\": \"CreateMLTransformRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The unique name that you give the transform when you create it.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of the machine learning transform that is being defined. The default is an empty string.\"\n        }\n      ]\n    },\n    \"InputRecordTables\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/GlueTables\"\n        },\n        {\n          \"description\": \"A list of Glue table definitions used by the transform.\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformParameters\"\n        },\n        {\n          \"description\": \"The algorithmic parameters that are specific to the transform type used. Conditionally dependent on the transform type.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleString\"\n        },\n        {\n          \"description\": \"<p>The name or Amazon Resource Name (ARN) of the IAM role with the required permissions. The required permissions include both Glue service role permissions to Glue resources, and Amazon S3 permissions required by the transform. </p> <ul> <li> <p>This role needs Glue service role permissions to allow access\
  \ to resources in Glue. See <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/attach-policy-iam-user.html\\\">Attach a Policy to IAM Users That Access Glue</a>.</p> </li> <li> <p>This role needs permission to your Amazon Simple Storage Service (Amazon S3) sources, targets, temporary directory, scripts, and any libraries used by the task run for this transform.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"GlueVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueVersionString\"\n        },\n        {\n          \"description\": \"This value determines which version of Glue this machine learning transform is compatible with. Glue 1.0 is recommended for most customers. If the value is not set, the Glue compatibility defaults to Glue 0.9. For more information, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/release-notes.html#release-notes-versions\\\">Glue Versions</a> in the developer guide.\"\n        }\n      ]\n    },\n   \
  \ \"MaxCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"<p>The number of Glue data processing units (DPUs) that are allocated to task runs for this transform. You can allocate from 2 to 100 DPUs; the default is 10. A DPU is a relative measure of processing power that consists of 4 vCPUs of compute capacity and 16 GB of memory. For more information, see the <a href=\\\"https://aws.amazon.com/glue/pricing/\\\">Glue pricing page</a>. </p> <p> <code>MaxCapacity</code> is a mutually exclusive option with <code>NumberOfWorkers</code> and <code>WorkerType</code>.</p> <ul> <li> <p>If either <code>NumberOfWorkers</code> or <code>WorkerType</code> is set, then <code>MaxCapacity</code> cannot be set.</p> </li> <li> <p>If <code>MaxCapacity</code> is set then neither <code>NumberOfWorkers</code> or <code>WorkerType</code> can be set.</p> </li> <li> <p>If <code>WorkerType</code> is set, then\
  \ <code>NumberOfWorkers</code> is required (and vice versa).</p> </li> <li> <p> <code>MaxCapacity</code> and <code>NumberOfWorkers</code> must both be at least 1.</p> </li> </ul> <p>When the <code>WorkerType</code> field is set to a value other than <code>Standard</code>, the <code>MaxCapacity</code> field is set automatically and becomes read-only.</p> <p>When the <code>WorkerType</code> field is set to a value other than <code>Standard</code>, the <code>MaxCapacity</code> field is set automatically and becomes read-only.</p>\"\n        }\n      ]\n    },\n    \"WorkerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkerType\"\n        },\n        {\n          \"description\": \"<p>The type of predefined worker that is allocated when this task runs. Accepts a value of Standard, G.1X, or G.2X.</p> <ul> <li> <p>For the <code>Standard</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 50GB disk, and 2 executors per worker.</p> </li>\
  \ <li> <p>For the <code>G.1X</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 64GB disk, and 1 executor per worker.</p> </li> <li> <p>For the <code>G.2X</code> worker type, each worker provides 8 vCPU, 32 GB of memory and a 128GB disk, and 1 executor per worker.</p> </li> </ul> <p> <code>MaxCapacity</code> is a mutually exclusive option with <code>NumberOfWorkers</code> and <code>WorkerType</code>.</p> <ul> <li> <p>If either <code>NumberOfWorkers</code> or <code>WorkerType</code> is set, then <code>MaxCapacity</code> cannot be set.</p> </li> <li> <p>If <code>MaxCapacity</code> is set then neither <code>NumberOfWorkers</code> or <code>WorkerType</code> can be set.</p> </li> <li> <p>If <code>WorkerType</code> is set, then <code>NumberOfWorkers</code> is required (and vice versa).</p> </li> <li> <p> <code>MaxCapacity</code> and <code>NumberOfWorkers</code> must both be at least 1.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p>The number of workers of a defined <code>workerType</code> that are allocated when this task runs.</p> <p>If <code>WorkerType</code> is set, then <code>NumberOfWorkers</code> is required (and vice versa).</p>\"\n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The timeout of the task run for this transform in minutes. This is the maximum time that a task run for this transform can consume resources before it is terminated and enters <code>TIMEOUT</code> status. The default is 2,880 minutes (48 hours).\"\n        }\n      ]\n    },\n    \"MaxRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The maximum number of times\
  \ to retry a task for this transform after a task run fails.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags to use with this machine learning transform. You may use tags to limit access to the machine learning transform. For more information about tags in Glue, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-tags.html\\\">Amazon Web Services Tags in Glue</a> in the developer guide.\"\n        }\n      ]\n    },\n    \"TransformEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformEncryption\"\n        },\n        {\n          \"description\": \"The encryption-at-rest settings of the transform that apply to accessing user data. Machine learning transforms can access user data encrypted in Amazon S3 using KMS.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n\
  \    \"InputRecordTables\",\n    \"Parameters\",\n    \"Role\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-ml-transform-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateMLTransformRequest
---
