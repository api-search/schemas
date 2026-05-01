---
description: CreateDevEndpointResponse schema from Amazon Glue API
layout: schema
name: CreateDevEndpointResponse
properties_list:
- description: ''
  name: EndpointName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: SubnetId
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: YarnEndpointAddress
  type: object
- description: ''
  name: ZeppelinRemoteSparkInterpreterPort
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
  name: AvailabilityZone
  type: object
- description: ''
  name: VpcId
  type: object
- description: ''
  name: ExtraPythonLibsS3Path
  type: object
- description: ''
  name: ExtraJarsS3Path
  type: object
- description: ''
  name: FailureReason
  type: object
- description: ''
  name: SecurityConfiguration
  type: object
- description: ''
  name: CreatedTimestamp
  type: object
- description: ''
  name: Arguments
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-dev-endpoint-response-schema.json
slug: glue-create-dev-endpoint-response
source_filename: glue-create-dev-endpoint-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-dev-endpoint-response-schema.json\",\n  \"title\": \"CreateDevEndpointResponse\",\n  \"description\": \"CreateDevEndpointResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name assigned to the new <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The current status of the new <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringList\"\
  \n        },\n        {\n          \"description\": \"The security groups assigned to the new <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The subnet ID assigned to the new <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the role assigned to the new <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"YarnEndpointAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The address of the YARN endpoint used by this <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"ZeppelinRemoteSparkInterpreterPort\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerValue\"\n        },\n        {\n          \"description\": \"The Apache Zeppelin port for the remote Apache Spark interpreter.\"\n        }\n      ]\n    },\n    \"NumberOfNodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerValue\"\n        },\n        {\n          \"description\": \"The number of Glue Data Processing Units (DPUs) allocated to this DevEndpoint.\"\n        }\n      ]\n    },\n    \"WorkerType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkerType\"\n        },\n        {\n          \"description\": \"The type of predefined worker that is allocated to the development endpoint. May be a value of Standard, G.1X, or G.2X.\"\n        }\n      ]\n    },\n    \"GlueVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GlueVersionString\"\n        },\n        {\n          \"description\"\
  : \"<p>Glue version determines the versions of Apache Spark and Python that Glue supports. The Python version indicates the version supported for running your ETL scripts on development endpoints. </p> <p>For more information about the available Glue versions and corresponding Spark and Python versions, see <a href=\\\"https://docs.aws.amazon.com/glue/latest/dg/add-job.html\\\">Glue version</a> in the developer guide.</p>\"\n        }\n      ]\n    },\n    \"NumberOfWorkers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"The number of workers of a defined <code>workerType</code> that are allocated to the development endpoint.\"\n        }\n      ]\n    },\n    \"AvailabilityZone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Availability Zone where this <code>DevEndpoint</code>\
  \ is located.\"\n        }\n      ]\n    },\n    \"VpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The ID of the virtual private cloud (VPC) used by this <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"ExtraPythonLibsS3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The paths to one or more Python libraries in an S3 bucket that will be loaded in your <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"ExtraJarsS3Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"Path to one or more Java <code>.jar</code> files in an S3 bucket that will be loaded in your <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"FailureReason\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The reason for a current failure in this <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"SecurityConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the <code>SecurityConfiguration</code> structure being used with this <code>DevEndpoint</code>.\"\n        }\n      ]\n    },\n    \"CreatedTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampValue\"\n        },\n        {\n          \"description\": \"The point in time at which this <code>DevEndpoint</code> was created.\"\n        }\n      ]\n    },\n    \"Arguments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapValue\"\n        },\n        {\n          \"description\": \"<p>The map of arguments used\
  \ to configure this <code>DevEndpoint</code>.</p> <p>Valid arguments are:</p> <ul> <li> <p> <code>\\\"--enable-glue-datacatalog\\\": \\\"\\\"</code> </p> </li> </ul> <p>You can specify a version of Python support for development endpoints by using the <code>Arguments</code> parameter in the <code>CreateDevEndpoint</code> or <code>UpdateDevEndpoint</code> APIs. If no arguments are provided, the version defaults to Python 2.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-dev-endpoint-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateDevEndpointResponse
---
