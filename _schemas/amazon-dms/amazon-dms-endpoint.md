---
description: <p>Describes an endpoint of a database instance in response to operations such as the following:</p> <ul> <li> <p> <code>CreateEndpoint</code> </p> </li> <li> <p> <code>DescribeEndpoint</code> </p> </li> <li> <p> <code>ModifyEndpoint</code> </p> </li> </ul>
layout: schema
name: Endpoint
properties_list:
- description: ''
  name: EndpointIdentifier
  type: object
- description: ''
  name: EndpointType
  type: object
- description: ''
  name: EngineName
  type: object
- description: ''
  name: EngineDisplayName
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: ServerName
  type: object
- description: ''
  name: Port
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: ExtraConnectionAttributes
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: KmsKeyId
  type: object
- description: ''
  name: EndpointArn
  type: object
- description: ''
  name: CertificateArn
  type: object
- description: ''
  name: SslMode
  type: object
- description: ''
  name: ServiceAccessRoleArn
  type: object
- description: ''
  name: ExternalTableDefinition
  type: object
- description: ''
  name: ExternalId
  type: object
- description: ''
  name: DynamoDbSettings
  type: object
- description: ''
  name: S3Settings
  type: object
- description: ''
  name: DmsTransferSettings
  type: object
- description: ''
  name: MongoDbSettings
  type: object
- description: ''
  name: KinesisSettings
  type: object
- description: ''
  name: KafkaSettings
  type: object
- description: ''
  name: ElasticsearchSettings
  type: object
- description: ''
  name: NeptuneSettings
  type: object
- description: ''
  name: RedshiftSettings
  type: object
- description: ''
  name: PostgreSQLSettings
  type: object
- description: ''
  name: MySQLSettings
  type: object
- description: ''
  name: OracleSettings
  type: object
- description: ''
  name: SybaseSettings
  type: object
- description: ''
  name: MicrosoftSQLServerSettings
  type: object
- description: ''
  name: IBMDb2Settings
  type: object
- description: ''
  name: DocDbSettings
  type: object
- description: ''
  name: RedisSettings
  type: object
- description: ''
  name: GcpMySQLSettings
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-endpoint-schema.json
slug: amazon-dms-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-endpoint-schema.json\",\n  \"title\": \"Endpoint\",\n  \"description\": \"<p>Describes an endpoint of a database instance in response to operations such as the following:</p> <ul> <li> <p> <code>CreateEndpoint</code> </p> </li> <li> <p> <code>DescribeEndpoint</code> </p> </li> <li> <p> <code>ModifyEndpoint</code> </p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndpointIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The database endpoint identifier. Identifiers must begin with a letter and must contain only ASCII letters, digits, and hyphens. They can't end with a hyphen or contain two consecutive hyphens.\"\n        }\n      ]\n    },\n    \"EndpointType\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReplicationEndpointTypeValue\"\n        },\n        {\n          \"description\": \"The type of endpoint. Valid values are <code>source</code> and <code>target</code>.\"\n        }\n      ]\n    },\n    \"EngineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The database engine name. Valid values, depending on the EndpointType, include <code>\\\"mysql\\\"</code>, <code>\\\"oracle\\\"</code>, <code>\\\"postgres\\\"</code>, <code>\\\"mariadb\\\"</code>, <code>\\\"aurora\\\"</code>, <code>\\\"aurora-postgresql\\\"</code>, <code>\\\"redshift\\\"</code>, <code>\\\"s3\\\"</code>, <code>\\\"db2\\\"</code>, <code>\\\"db2-zos\\\"</code>, <code>\\\"azuredb\\\"</code>, <code>\\\"sybase\\\"</code>, <code>\\\"dynamodb\\\"</code>, <code>\\\"mongodb\\\"</code>, <code>\\\"kinesis\\\"</code>, <code>\\\"kafka\\\"</code>, <code>\\\"elasticsearch\\\
  \"</code>, <code>\\\"documentdb\\\"</code>, <code>\\\"sqlserver\\\"</code>, <code>\\\"neptune\\\"</code>, and <code>\\\"babelfish\\\"</code>.\"\n        }\n      ]\n    },\n    \"EngineDisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The expanded name for the engine name. For example, if the <code>EngineName</code> parameter is \\\"aurora\\\", this value would be \\\"Amazon Aurora MySQL\\\".\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The user name used to connect to the endpoint.\"\n        }\n      ]\n    },\n    \"ServerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the server at the endpoint.\"\n        }\n      ]\n    },\n   \
  \ \"Port\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerOptional\"\n        },\n        {\n          \"description\": \"The port value used to access the endpoint.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the database at the endpoint.\"\n        }\n      ]\n    },\n    \"ExtraConnectionAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Additional connection attributes used to connect to the endpoint.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status of the endpoint.\"\n        }\n      ]\n    },\n    \"KmsKeyId\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>An KMS key identifier that is used to encrypt the connection parameters for the endpoint.</p> <p>If you don't specify a value for the <code>KmsKeyId</code> parameter, then DMS uses your default encryption key.</p> <p>KMS creates the default encryption key for your Amazon Web Services account. Your Amazon Web Services account has a different default encryption key for each Amazon Web Services Region.</p>\"\n        }\n      ]\n    },\n    \"EndpointArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) string that uniquely identifies the endpoint.\"\n        }\n      ]\n    },\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource\
  \ Name (ARN) used for SSL connection to the endpoint.\"\n        }\n      ]\n    },\n    \"SslMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DmsSslModeValue\"\n        },\n        {\n          \"description\": \"The SSL mode used to connect to the endpoint. The default value is <code>none</code>.\"\n        }\n      ]\n    },\n    \"ServiceAccessRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) used by the service to access the IAM role. The role must allow the <code>iam:PassRole</code> action.\"\n        }\n      ]\n    },\n    \"ExternalTableDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The external table definition.\"\n        }\n      ]\n    },\n    \"ExternalId\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" Value returned by a call to CreateEndpoint that can be used for cross-account validation. Use it on a subsequent call to CreateEndpoint to create the endpoint with a cross-account. \"\n        }\n      ]\n    },\n    \"DynamoDbSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DynamoDbSettings\"\n        },\n        {\n          \"description\": \"The settings for the DynamoDB target endpoint. For more information, see the <code>DynamoDBSettings</code> structure.\"\n        }\n      ]\n    },\n    \"S3Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Settings\"\n        },\n        {\n          \"description\": \"The settings for the S3 target endpoint. For more information, see the <code>S3Settings</code> structure.\"\n        }\n      ]\n    },\n    \"DmsTransferSettings\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/DmsTransferSettings\"\n        },\n        {\n          \"description\": \"The settings for the DMS Transfer type source. For more information, see the DmsTransferSettings structure. \"\n        }\n      ]\n    },\n    \"MongoDbSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MongoDbSettings\"\n        },\n        {\n          \"description\": \"The settings for the MongoDB source endpoint. For more information, see the <code>MongoDbSettings</code> structure.\"\n        }\n      ]\n    },\n    \"KinesisSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisSettings\"\n        },\n        {\n          \"description\": \"The settings for the Amazon Kinesis target endpoint. For more information, see the <code>KinesisSettings</code> structure.\"\n        }\n      ]\n    },\n    \"KafkaSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KafkaSettings\"\
  \n        },\n        {\n          \"description\": \"The settings for the Apache Kafka target endpoint. For more information, see the <code>KafkaSettings</code> structure.\"\n        }\n      ]\n    },\n    \"ElasticsearchSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchSettings\"\n        },\n        {\n          \"description\": \"The settings for the OpenSearch source endpoint. For more information, see the <code>ElasticsearchSettings</code> structure.\"\n        }\n      ]\n    },\n    \"NeptuneSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NeptuneSettings\"\n        },\n        {\n          \"description\": \"The settings for the Amazon Neptune target endpoint. For more information, see the <code>NeptuneSettings</code> structure.\"\n        }\n      ]\n    },\n    \"RedshiftSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedshiftSettings\"\n    \
  \    },\n        {\n          \"description\": \"Settings for the Amazon Redshift endpoint.\"\n        }\n      ]\n    },\n    \"PostgreSQLSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PostgreSQLSettings\"\n        },\n        {\n          \"description\": \"The settings for the PostgreSQL source and target endpoint. For more information, see the <code>PostgreSQLSettings</code> structure.\"\n        }\n      ]\n    },\n    \"MySQLSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MySQLSettings\"\n        },\n        {\n          \"description\": \"The settings for the MySQL source and target endpoint. For more information, see the <code>MySQLSettings</code> structure.\"\n        }\n      ]\n    },\n    \"OracleSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OracleSettings\"\n        },\n        {\n          \"description\": \"The settings for the Oracle source and target\
  \ endpoint. For more information, see the <code>OracleSettings</code> structure.\"\n        }\n      ]\n    },\n    \"SybaseSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SybaseSettings\"\n        },\n        {\n          \"description\": \"The settings for the SAP ASE source and target endpoint. For more information, see the <code>SybaseSettings</code> structure.\"\n        }\n      ]\n    },\n    \"MicrosoftSQLServerSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MicrosoftSQLServerSettings\"\n        },\n        {\n          \"description\": \"The settings for the Microsoft SQL Server source and target endpoint. For more information, see the <code>MicrosoftSQLServerSettings</code> structure.\"\n        }\n      ]\n    },\n    \"IBMDb2Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IBMDb2Settings\"\n        },\n        {\n          \"description\": \"The settings\
  \ for the IBM Db2 LUW source endpoint. For more information, see the <code>IBMDb2Settings</code> structure. \"\n        }\n      ]\n    },\n    \"DocDbSettings\": {\n      \"$ref\": \"#/components/schemas/DocDbSettings\"\n    },\n    \"RedisSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RedisSettings\"\n        },\n        {\n          \"description\": \"The settings for the Redis target endpoint. For more information, see the <code>RedisSettings</code> structure.\"\n        }\n      ]\n    },\n    \"GcpMySQLSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GcpMySQLSettings\"\n        },\n        {\n          \"description\": \"Settings in JSON format for the source GCP MySQL endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-endpoint-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: Endpoint
---
