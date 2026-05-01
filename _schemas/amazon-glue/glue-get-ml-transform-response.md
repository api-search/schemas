---
description: GetMLTransformResponse schema from Amazon Glue API
layout: schema
name: GetMLTransformResponse
properties_list:
- description: ''
  name: TransformId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreatedOn
  type: object
- description: ''
  name: LastModifiedOn
  type: object
- description: ''
  name: InputRecordTables
  type: object
- description: ''
  name: Parameters
  type: object
- description: ''
  name: EvaluationMetrics
  type: object
- description: ''
  name: LabelCount
  type: object
- description: ''
  name: Schema
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
  name: TransformEncryption
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-ml-transform-response-schema.json
slug: glue-get-ml-transform-response
source_filename: glue-get-ml-transform-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-transform-response-schema.json\",\n  \"title\": \"GetMLTransformResponse\",\n  \"description\": \"GetMLTransformResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the transform, generated at the time that the transform was created.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The unique name given to the transform when it was created.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"A description of the transform.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformStatusType\"\n        },\n        {\n          \"description\": \"The last known status of the transform (to indicate whether it can be used or not). One of \\\"NOT_READY\\\", \\\"READY\\\", or \\\"DELETING\\\".\"\n        }\n      ]\n    },\n    \"CreatedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the transform was created.\"\n        }\n      ]\n    },\n    \"LastModifiedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the transform was last modified.\"\n        }\n      ]\n    },\n\
  \    \"InputRecordTables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueTables\"\n        },\n        {\n          \"description\": \"A list of Glue table definitions used by the transform.\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformParameters\"\n        },\n        {\n          \"description\": \"The configuration parameters that are specific to the algorithm used.\"\n        }\n      ]\n    },\n    \"EvaluationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EvaluationMetrics\"\n        },\n        {\n          \"description\": \"The latest evaluation metrics.\"\n        }\n      ]\n    },\n    \"LabelCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LabelCount\"\n        },\n        {\n          \"description\": \"The number of labels available for this transform.\"\n        }\n \
  \     ]\n    },\n    \"Schema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformSchema\"\n        },\n        {\n          \"description\": \"The <code>Map&lt;Column, Type&gt;</code> object that represents the schema that this transform accepts. Has an upper bound of 100 columns.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleString\"\n        },\n        {\n          \"description\": \"The name or Amazon Resource Name (ARN) of the IAM role with the required permissions.\"\n        }\n      ]\n    },\n    \"GlueVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueVersionString\"\n        },\n        {\n          \"description\": \"This value determines which version of Glue this machine learning transform is compatible with. Glue 1.0 is recommended for most customers. If the value is not set, the Glue compatibility defaults to Glue\
  \ 0.9. For more information, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/release-notes.html#release-notes-versions\\\">Glue Versions</a> in the developer guide.\"\n        }\n      ]\n    },\n    \"MaxCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableDouble\"\n        },\n        {\n          \"description\": \"<p>The number of Glue data processing units (DPUs) that are allocated to task runs for this transform. You can allocate from 2 to 100 DPUs; the default is 10. A DPU is a relative measure of processing power that consists of 4 vCPUs of compute capacity and 16 GB of memory. For more information, see the <a href=\\\"https://aws.amazon.com/glue/pricing/\\\">Glue pricing page</a>. </p> <p>When the <code>WorkerType</code> field is set to a value other than <code>Standard</code>, the <code>MaxCapacity</code> field is set automatically and becomes read-only.</p>\"\n        }\n      ]\n    },\n    \"WorkerType\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/WorkerType\"\n        },\n        {\n          \"description\": \"<p>The type of predefined worker that is allocated when this task runs. Accepts a value of Standard, G.1X, or G.2X.</p> <ul> <li> <p>For the <code>Standard</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 50GB disk, and 2 executors per worker.</p> </li> <li> <p>For the <code>G.1X</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 64GB disk, and 1 executor per worker.</p> </li> <li> <p>For the <code>G.2X</code> worker type, each worker provides 8 vCPU, 32 GB of memory and a 128GB disk, and 1 executor per worker.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of workers of a defined <code>workerType</code> that are allocated when this task runs.\"\
  \n        }\n      ]\n    },\n    \"Timeout\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timeout\"\n        },\n        {\n          \"description\": \"The timeout for a task run for this transform in minutes. This is the maximum time that a task run for this transform can consume resources before it is terminated and enters <code>TIMEOUT</code> status. The default is 2,880 minutes (48 hours).\"\n        }\n      ]\n    },\n    \"MaxRetries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The maximum number of times to retry a task for this transform after a task run fails.\"\n        }\n      ]\n    },\n    \"TransformEncryption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformEncryption\"\n        },\n        {\n          \"description\": \"The encryption-at-rest settings of the transform that apply to accessing\
  \ user data. Machine learning transforms can access user data encrypted in Amazon S3 using KMS.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-transform-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMLTransformResponse
---
