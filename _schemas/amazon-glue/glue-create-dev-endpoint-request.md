---
description: CreateDevEndpointRequest schema from Amazon Glue API
layout: schema
name: CreateDevEndpointRequest
properties_list:
- description: ''
  name: EndpointName
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: PublicKey
  type: object
- description: ''
  name: PublicKeys
  type: object
- description: ''
  name: NumberOfNodes
  type: object
- description: ''
  name: WorkerType
  type: object
- description: ''
  name: GlueVersion
  type: object
- description: ''
  name: NumberOfWorkers
  type: object
- description: ''
  name: ExtraPythonLibsS3Path
  type: object
- description: ''
  name: ExtraJarsS3Path
  type: object
- description: ''
  name: SecurityConfiguration
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Arguments
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-dev-endpoint-request-schema.json
slug: glue-create-dev-endpoint-request
source_filename: glue-create-dev-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-dev-endpoint-request-schema.json\",\n  \"title\": \"CreateDevEndpointRequest\",\n  \"description\": \"CreateDevEndpointRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name to be assigned to the new <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The IAM role for the <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\
  \n        },\n        {\n          \"description\": \"Security group IDs for the security groups to be used by the new <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The subnet ID for the new <code>DevEndpoint</code> to use.\"\n        }\n      ]\n    },\n    \"PublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The public key to be used by this <code>DevEndpoint</code> for authentication. This attribute is provided for backward compatibility because the recommended attribute to use is public keys.\"\n        }\n      ]\n    },\n    \"PublicKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublicKeysList\"\n        },\n        {\n          \"description\": \"<p>A list of public\
  \ keys to be used by the development endpoints for authentication. The use of this attribute is preferred over a single public key because the public keys allow you to have a different private key per client.</p> <note> <p>If you previously created an endpoint with a public key, you must remove that key to be able to set a list of public keys. Call the <code>UpdateDevEndpoint</code> API with the public key content in the <code>deletePublicKeys</code> attribute, and the list of new keys in the <code>addPublicKeys</code> attribute.</p> </note>\"\n        }\n      ]\n    },\n    \"NumberOfNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerValue\"\n        },\n        {\n          \"description\": \"The number of Glue Data Processing Units (DPUs) to allocate to this <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"WorkerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkerType\"\n        },\n    \
  \    {\n          \"description\": \"<p>The type of predefined worker that is allocated to the development endpoint. Accepts a value of Standard, G.1X, or G.2X.</p> <ul> <li> <p>For the <code>Standard</code> worker type, each worker provides 4 vCPU, 16 GB of memory and a 50GB disk, and 2 executors per worker.</p> </li> <li> <p>For the <code>G.1X</code> worker type, each worker maps to 1 DPU (4 vCPU, 16 GB of memory, 64 GB disk), and provides 1 executor per worker. We recommend this worker type for memory-intensive jobs.</p> </li> <li> <p>For the <code>G.2X</code> worker type, each worker maps to 2 DPU (8 vCPU, 32 GB of memory, 128 GB disk), and provides 1 executor per worker. We recommend this worker type for memory-intensive jobs.</p> </li> </ul> <p>Known issue: when a development endpoint is created with the <code>G.2X</code> <code>WorkerType</code> configuration, the Spark drivers for the development endpoint will run on 4 vCPU, 16 GB of memory, and a 64 GB disk. </p>\"\n        }\n\
  \      ]\n    },\n    \"GlueVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueVersionString\"\n        },\n        {\n          \"description\": \"<p>Glue version determines the versions of Apache Spark and Python that Glue supports. The Python version indicates the version supported for running your ETL scripts on development endpoints. </p> <p>For more information about the available Glue versions and corresponding Spark and Python versions, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/add-job.html\\\">Glue version</a> in the developer guide.</p> <p>Development endpoints that are created without specifying a Glue version default to Glue 0.9.</p> <p>You can specify a version of Python support for development endpoints by using the <code>Arguments</code> parameter in the <code>CreateDevEndpoint</code> or <code>UpdateDevEndpoint</code> APIs. If no arguments are provided, the version defaults to Python 2.</p>\"\n        }\n      ]\n\
  \    },\n    \"NumberOfWorkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"<p>The number of workers of a defined <code>workerType</code> that are allocated to the development endpoint.</p> <p>The maximum number of workers you can define are 299 for <code>G.1X</code>, and 149 for <code>G.2X</code>. </p>\"\n        }\n      ]\n    },\n    \"ExtraPythonLibsS3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"<p>The paths to one or more Python libraries in an Amazon S3 bucket that should be loaded in your <code>DevEndpoint</code>. Multiple values must be complete paths separated by a comma.</p> <note> <p>You can only use pure Python libraries with a <code>DevEndpoint</code>. Libraries that rely on C extensions, such as the <a href=\\\"http://pandas.pydata.org/\\\">pandas</a> Python data\
  \ analysis library, are not yet supported.</p> </note>\"\n        }\n      ]\n    },\n    \"ExtraJarsS3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The path to one or more Java <code>.jar</code> files in an S3 bucket that should be loaded in your <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"SecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the <code>SecurityConfiguration</code> structure to be used with this <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"The tags to use with this DevEndpoint. You may use tags to limit access to the DevEndpoint. For more information about tags\
  \ in Glue, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/monitor-tags.html\\\">Amazon Web Services Tags in Glue</a> in the developer guide.\"\n        }\n      ]\n    },\n    \"Arguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapValue\"\n        },\n        {\n          \"description\": \"A map of arguments used to configure the <code>DevEndpoint</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"EndpointName\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-dev-endpoint-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateDevEndpointRequest
---
