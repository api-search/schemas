---
description: GetPartitionsRequest schema from Amazon Glue API
layout: schema
name: GetPartitionsRequest
properties_list:
- description: ''
  name: CatalogId
  type: object
- description: ''
  name: DatabaseName
  type: object
- description: ''
  name: TableName
  type: object
- description: ''
  name: Expression
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Segment
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: ExcludeColumnSchema
  type: object
- description: ''
  name: TransactionId
  type: object
- description: ''
  name: QueryAsOfTime
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-partitions-request-schema.json
slug: glue-get-partitions-request
source_filename: glue-get-partitions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partitions-request-schema.json\",\n  \"title\": \"GetPartitionsRequest\",\n  \"description\": \"GetPartitionsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CatalogId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CatalogIdString\"\n        },\n        {\n          \"description\": \"The ID of the Data Catalog where the partitions in question reside. If none is provided, the Amazon Web Services account ID is used by default.\"\n        }\n      ]\n    },\n    \"DatabaseName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the catalog database where the partitions reside.\"\n        }\n      ]\n    },\n    \"TableName\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the partitions' table.\"\n        }\n      ]\n    },\n    \"Expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PredicateString\"\n        },\n        {\n          \"description\": \"<p>An expression that filters the partitions to be returned.</p> <p>The expression uses SQL syntax similar to the SQL <code>WHERE</code> filter clause. The SQL statement parser <a href=\\\"http://jsqlparser.sourceforge.net/home.php\\\">JSQLParser</a> parses the expression. </p> <p> <i>Operators</i>: The following are the operators that you can use in the <code>Expression</code> API call:</p> <dl> <dt>=</dt> <dd> <p>Checks whether the values of the two operands are equal; if yes, then the condition becomes true.</p> <p>Example: Assume 'variable a' holds 10 and 'variable b' holds 20. </p> <p>(a = b) is not true.</p>\
  \ </dd> <dt>&lt; &gt;</dt> <dd> <p>Checks whether the values of two operands are equal; if the values are not equal, then the condition becomes true.</p> <p>Example: (a &lt; &gt; b) is true.</p> </dd> <dt>&gt;</dt> <dd> <p>Checks whether the value of the left operand is greater than the value of the right operand; if yes, then the condition becomes true.</p> <p>Example: (a &gt; b) is not true.</p> </dd> <dt>&lt;</dt> <dd> <p>Checks whether the value of the left operand is less than the value of the right operand; if yes, then the condition becomes true.</p> <p>Example: (a &lt; b) is true.</p> </dd> <dt>&gt;=</dt> <dd> <p>Checks whether the value of the left operand is greater than or equal to the value of the right operand; if yes, then the condition becomes true.</p> <p>Example: (a &gt;= b) is not true.</p> </dd> <dt>&lt;=</dt> <dd> <p>Checks whether the value of the left operand is less than or equal to the value of the right operand; if yes, then the condition becomes true.</p> <p>Example:\
  \ (a &lt;= b) is true.</p> </dd> <dt>AND, OR, IN, BETWEEN, LIKE, NOT, IS NULL</dt> <dd> <p>Logical operators.</p> </dd> </dl> <p> <i>Supported Partition Key Types</i>: The following are the supported partition keys.</p> <ul> <li> <p> <code>string</code> </p> </li> <li> <p> <code>date</code> </p> </li> <li> <p> <code>timestamp</code> </p> </li> <li> <p> <code>int</code> </p> </li> <li> <p> <code>bigint</code> </p> </li> <li> <p> <code>long</code> </p> </li> <li> <p> <code>tinyint</code> </p> </li> <li> <p> <code>smallint</code> </p> </li> <li> <p> <code>decimal</code> </p> </li> </ul> <p>If an type is encountered that is not valid, an exception is thrown. </p> <p>The following list shows the valid operators on each type. When you define a crawler, the <code>partitionKey</code> type is created as a <code>STRING</code>, to be compatible with the catalog partitions. </p> <p> <i>Sample API Call</i>: </p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"A continuation token, if this is not the first call to retrieve these partitions.\"\n        }\n      ]\n    },\n    \"Segment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Segment\"\n        },\n        {\n          \"description\": \"The segment of the table's partitions to scan in this request.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of partitions to return in a single response.\"\n        }\n      ]\n    },\n    \"ExcludeColumnSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanNullable\"\n        },\n        {\n          \"description\": \"When true, specifies not returning the partition column schema. Useful when you are interested only\
  \ in other partition attributes such as partition values or location. This approach avoids the problem of a large response by not returning duplicate data.\"\n        }\n      ]\n    },\n    \"TransactionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransactionIdString\"\n        },\n        {\n          \"description\": \"The transaction ID at which to read the partition contents.\"\n        }\n      ]\n    },\n    \"QueryAsOfTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time as of when to read the partition contents. If not set, the most recent transaction commit time will be used. Cannot be specified along with <code>TransactionId</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DatabaseName\",\n    \"TableName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-partitions-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetPartitionsRequest
---
