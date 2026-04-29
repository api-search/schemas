---
description: Represents an Amazon DynamoDB table with its associated configuration, key schema, throughput settings, indexes, and metadata.
layout: schema
name: Amazon DynamoDB Table
properties_list:
- description: The name of the table
  name: tableName
  type: string
- description: The Amazon Resource Name (ARN) that uniquely identifies the table
  name: tableArn
  type: string
- description: Unique identifier for the table
  name: tableId
  type: string
- description: The current state of the table
  name: tableStatus
  type: string
- description: The date and time when the table was created
  name: creationDateTime
  type: string
- description: The primary key structure for the table, consisting of one or two key elements
  name: keySchema
  type: array
- description: An array of attributes that describe the key schema for the table and indexes
  name: attributeDefinitions
  type: array
- description: ''
  name: provisionedThroughput
  type: object
- description: Controls how you are charged for read and write throughput
  name: billingMode
  type: string
- description: The number of items in the table (updated approximately every six hours)
  name: itemCount
  type: integer
- description: The total size of the table in bytes (updated approximately every six hours)
  name: tableSizeBytes
  type: integer
- description: The global secondary indexes, if any, on the table
  name: globalSecondaryIndexes
  type: array
- description: The local secondary indexes, if any, on the table
  name: localSecondaryIndexes
  type: array
- description: ''
  name: streamSpecification
  type: object
- description: ''
  name: sseDescription
  type: object
- description: Tags assigned to the table
  name: tags
  type: array
provider_name: Amazon DynamoDB
provider_slug: amazon-dynamodb
schema_file: json-schema/amazon-dynamodb-table-schema.json
slug: amazon-dynamodb-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/dynamodb/table.json\",\n  \"title\": \"Amazon DynamoDB Table\",\n  \"description\": \"Represents an Amazon DynamoDB table with its associated configuration, key schema, throughput settings, indexes, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"tableName\", \"keySchema\", \"attributeDefinitions\"],\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table\",\n      \"minLength\": 3,\n      \"maxLength\": 255,\n      \"pattern\": \"^[a-zA-Z0-9._-]+$\"\n    },\n    \"tableArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) that uniquely identifies the table\",\n      \"pattern\": \"^arn:aws:dynamodb:.+:\\\\d{12}:table/.+$\"\n    },\n    \"tableId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the table\"\
  ,\n      \"pattern\": \"^[a-f0-9-]{36}$\"\n    },\n    \"tableStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the table\",\n      \"enum\": [\"CREATING\", \"UPDATING\", \"DELETING\", \"ACTIVE\", \"INACCESSIBLE_ENCRYPTION_CREDENTIALS\", \"ARCHIVING\", \"ARCHIVED\"]\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time when the table was created\"\n    },\n    \"keySchema\": {\n      \"type\": \"array\",\n      \"description\": \"The primary key structure for the table, consisting of one or two key elements\",\n      \"items\": {\n        \"$ref\": \"#/$defs/KeySchemaElement\"\n      },\n      \"minItems\": 1,\n      \"maxItems\": 2\n    },\n    \"attributeDefinitions\": {\n      \"type\": \"array\",\n      \"description\": \"An array of attributes that describe the key schema for the table and indexes\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AttributeDefinition\"\
  \n      }\n    },\n    \"provisionedThroughput\": {\n      \"$ref\": \"#/$defs/ProvisionedThroughput\"\n    },\n    \"billingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Controls how you are charged for read and write throughput\",\n      \"enum\": [\"PROVISIONED\", \"PAY_PER_REQUEST\"]\n    },\n    \"itemCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of items in the table (updated approximately every six hours)\",\n      \"minimum\": 0\n    },\n    \"tableSizeBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"The total size of the table in bytes (updated approximately every six hours)\",\n      \"minimum\": 0\n    },\n    \"globalSecondaryIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"The global secondary indexes, if any, on the table\",\n      \"items\": {\n        \"$ref\": \"#/$defs/GlobalSecondaryIndex\"\n      }\n    },\n    \"localSecondaryIndexes\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"The local secondary indexes, if any, on the table\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LocalSecondaryIndex\"\n      }\n    },\n    \"streamSpecification\": {\n      \"$ref\": \"#/$defs/StreamSpecification\"\n    },\n    \"sseDescription\": {\n      \"$ref\": \"#/$defs/SSEDescription\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the table\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"KeySchemaElement\": {\n      \"type\": \"object\",\n      \"description\": \"Represents a single element of a key schema, specifying the attribute name and its role\",\n      \"required\": [\"attributeName\", \"keyType\"],\n      \"properties\": {\n        \"attributeName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of a key attribute\"\n        },\n        \"keyType\": {\n          \"type\": \"string\",\n          \"description\": \"The role that this\
  \ key attribute will assume (HASH for partition key, RANGE for sort key)\",\n          \"enum\": [\"HASH\", \"RANGE\"]\n        }\n      }\n    },\n    \"AttributeDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"Represents an attribute for describing the key schema for the table and indexes\",\n      \"required\": [\"attributeName\", \"attributeType\"],\n      \"properties\": {\n        \"attributeName\": {\n          \"type\": \"string\",\n          \"description\": \"A name for the attribute\"\n        },\n        \"attributeType\": {\n          \"type\": \"string\",\n          \"description\": \"The data type for the attribute (S=String, N=Number, B=Binary)\",\n          \"enum\": [\"S\", \"N\", \"B\"]\n        }\n      }\n    },\n    \"ProvisionedThroughput\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the provisioned throughput settings for the table\",\n      \"properties\": {\n        \"readCapacityUnits\": {\n          \"type\": \"\
  integer\",\n          \"description\": \"The maximum number of strongly consistent reads consumed per second\",\n          \"minimum\": 1\n        },\n        \"writeCapacityUnits\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of writes consumed per second\",\n          \"minimum\": 1\n        },\n        \"lastIncreaseDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time of the last provisioned throughput increase\"\n        },\n        \"lastDecreaseDateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time of the last provisioned throughput decrease\"\n        },\n        \"numberOfDecreasesToday\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of provisioned throughput decreases for this table during this UTC calendar day\",\n          \"minimum\": 0\n        }\n\
  \      }\n    },\n    \"GlobalSecondaryIndex\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the properties of a global secondary index\",\n      \"required\": [\"indexName\", \"keySchema\", \"projection\"],\n      \"properties\": {\n        \"indexName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the global secondary index\",\n          \"minLength\": 3,\n          \"maxLength\": 255\n        },\n        \"keySchema\": {\n          \"type\": \"array\",\n          \"description\": \"The complete key schema for the global secondary index\",\n          \"items\": {\n            \"$ref\": \"#/$defs/KeySchemaElement\"\n          },\n          \"minItems\": 1,\n          \"maxItems\": 2\n        },\n        \"projection\": {\n          \"$ref\": \"#/$defs/Projection\"\n        },\n        \"indexStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The current state of the global secondary index\",\n          \"\
  enum\": [\"CREATING\", \"UPDATING\", \"DELETING\", \"ACTIVE\"]\n        },\n        \"provisionedThroughput\": {\n          \"$ref\": \"#/$defs/ProvisionedThroughput\"\n        },\n        \"indexSizeBytes\": {\n          \"type\": \"integer\",\n          \"description\": \"The total size of the index in bytes\",\n          \"minimum\": 0\n        },\n        \"itemCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of items in the index\",\n          \"minimum\": 0\n        },\n        \"indexArn\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Resource Name (ARN) of the index\"\n        }\n      }\n    },\n    \"LocalSecondaryIndex\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the properties of a local secondary index\",\n      \"required\": [\"indexName\", \"keySchema\", \"projection\"],\n      \"properties\": {\n        \"indexName\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The name of the local secondary index\",\n          \"minLength\": 3,\n          \"maxLength\": 255\n        },\n        \"keySchema\": {\n          \"type\": \"array\",\n          \"description\": \"The complete key schema for the local secondary index\",\n          \"items\": {\n            \"$ref\": \"#/$defs/KeySchemaElement\"\n          },\n          \"minItems\": 2,\n          \"maxItems\": 2\n        },\n        \"projection\": {\n          \"$ref\": \"#/$defs/Projection\"\n        },\n        \"indexSizeBytes\": {\n          \"type\": \"integer\",\n          \"description\": \"The total size of the index in bytes\",\n          \"minimum\": 0\n        },\n        \"itemCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of items in the index\",\n          \"minimum\": 0\n        },\n        \"indexArn\": {\n          \"type\": \"string\",\n          \"description\": \"The Amazon Resource Name (ARN) of the index\"\n        }\n      }\n    },\n\
  \    \"Projection\": {\n      \"type\": \"object\",\n      \"description\": \"Represents attributes that are copied from the table into an index\",\n      \"properties\": {\n        \"projectionType\": {\n          \"type\": \"string\",\n          \"description\": \"The set of attributes that are projected into the index\",\n          \"enum\": [\"ALL\", \"KEYS_ONLY\", \"INCLUDE\"]\n        },\n        \"nonKeyAttributes\": {\n          \"type\": \"array\",\n          \"description\": \"The non-key attributes that are projected into the index\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"maxItems\": 20\n        }\n      }\n    },\n    \"StreamSpecification\": {\n      \"type\": \"object\",\n      \"description\": \"Represents the DynamoDB Streams configuration for the table\",\n      \"properties\": {\n        \"streamEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Indicates whether DynamoDB Streams is enabled on the\
  \ table\"\n        },\n        \"streamViewType\": {\n          \"type\": \"string\",\n          \"description\": \"Determines the information that is written to the stream\",\n          \"enum\": [\"KEYS_ONLY\", \"NEW_IMAGE\", \"OLD_IMAGE\", \"NEW_AND_OLD_IMAGES\"]\n        }\n      }\n    },\n    \"SSEDescription\": {\n      \"type\": \"object\",\n      \"description\": \"The description of the server-side encryption status on the table\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The current state of server-side encryption\",\n          \"enum\": [\"ENABLING\", \"ENABLED\", \"DISABLING\", \"DISABLED\", \"UPDATING\"]\n        },\n        \"sseType\": {\n          \"type\": \"string\",\n          \"description\": \"Server-side encryption type\",\n          \"enum\": [\"AES256\", \"KMS\"]\n        },\n        \"kmsMasterKeyArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the KMS key used\
  \ for SSE-KMS encryption\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a resource tag\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag\",\n          \"maxLength\": 128\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag\",\n          \"maxLength\": 256\n        }\n      },\n      \"required\": [\"key\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dynamodb/refs/heads/main/json-schema/amazon-dynamodb-table-schema.json
tags:
- AWS
- Database
- Document Store
- Key-Value
- NoSQL
- Serverless
title: Amazon DynamoDB Table
---
