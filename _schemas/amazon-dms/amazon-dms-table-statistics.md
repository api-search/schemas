---
description: Provides a collection of table statistics in response to a request by the <code>DescribeTableStatistics</code> operation.
layout: schema
name: TableStatistics
properties_list:
- description: ''
  name: SchemaName
  type: object
- description: ''
  name: TableName
  type: object
- description: ''
  name: Inserts
  type: object
- description: ''
  name: Deletes
  type: object
- description: ''
  name: Updates
  type: object
- description: ''
  name: Ddls
  type: object
- description: ''
  name: AppliedInserts
  type: object
- description: ''
  name: AppliedDeletes
  type: object
- description: ''
  name: AppliedUpdates
  type: object
- description: ''
  name: AppliedDdls
  type: object
- description: ''
  name: FullLoadRows
  type: object
- description: ''
  name: FullLoadCondtnlChkFailedRows
  type: object
- description: ''
  name: FullLoadErrorRows
  type: object
- description: ''
  name: FullLoadStartTime
  type: object
- description: ''
  name: FullLoadEndTime
  type: object
- description: ''
  name: FullLoadReloaded
  type: object
- description: ''
  name: LastUpdateTime
  type: object
- description: ''
  name: TableState
  type: object
- description: ''
  name: ValidationPendingRecords
  type: object
- description: ''
  name: ValidationFailedRecords
  type: object
- description: ''
  name: ValidationSuspendedRecords
  type: object
- description: ''
  name: ValidationState
  type: object
- description: ''
  name: ValidationStateDetails
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-table-statistics-schema.json
slug: amazon-dms-table-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-table-statistics-schema.json\",\n  \"title\": \"TableStatistics\",\n  \"description\": \"Provides a collection of table statistics in response to a request by the <code>DescribeTableStatistics</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SchemaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The schema name.\"\n        }\n      ]\n    },\n    \"TableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the table.\"\n        }\n      ]\n    },\n    \"Inserts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n \
  \         \"description\": \"The number of insert actions performed on a table.\"\n        }\n      ]\n    },\n    \"Deletes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of delete actions performed on a table.\"\n        }\n      ]\n    },\n    \"Updates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of update actions performed on a table.\"\n        }\n      ]\n    },\n    \"Ddls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The data definition language (DDL) used to build and modify the structure of your tables.\"\n        }\n      ]\n    },\n    \"AppliedInserts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n    \
  \      \"description\": \"The number of insert actions applied on a target table.\"\n        }\n      ]\n    },\n    \"AppliedDeletes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n          \"description\": \"The number of delete actions applied on a target table.\"\n        }\n      ]\n    },\n    \"AppliedUpdates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n          \"description\": \"The number of update actions applied on a target table.\"\n        }\n      ]\n    },\n    \"AppliedDdls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongOptional\"\n        },\n        {\n          \"description\": \"The number of data definition language (DDL) statements used to build and modify the structure of your tables applied on the target.\"\n        }\n      ]\n    },\n    \"FullLoadRows\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of rows added during the full load operation.\"\n        }\n      ]\n    },\n    \"FullLoadCondtnlChkFailedRows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of rows that failed conditional checks during the full load operation (valid only for migrations where DynamoDB is the target).\"\n        }\n      ]\n    },\n    \"FullLoadErrorRows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of rows that failed to load during the full load operation (valid only for migrations where DynamoDB is the target).\"\n        }\n      ]\n    },\n    \"FullLoadStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n  \
  \      {\n          \"description\": \"The time when the full load operation started.\"\n        }\n      ]\n    },\n    \"FullLoadEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The time when the full load operation completed.\"\n        }\n      ]\n    },\n    \"FullLoadReloaded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanOptional\"\n        },\n        {\n          \"description\": \"A value that indicates if the table was reloaded (<code>true</code>) or loaded as part of a new full load operation (<code>false</code>).\"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TStamp\"\n        },\n        {\n          \"description\": \"The last time a table was updated.\"\n        }\n      ]\n    },\n    \"TableState\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The state of the tables described.</p> <p>Valid states: Table does not exist | Before load | Full load | Table completed | Table cancelled | Table error | Table is being reloaded</p>\"\n        }\n      ]\n    },\n    \"ValidationPendingRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of records that have yet to be validated.\"\n        }\n      ]\n    },\n    \"ValidationFailedRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of records that failed validation.\"\n        }\n      ]\n    },\n    \"ValidationSuspendedRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The number of records\
  \ that couldn't be validated.\"\n        }\n      ]\n    },\n    \"ValidationState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The validation state of the table.</p> <p>This parameter can have the following values:</p> <ul> <li> <p>Not enabled \\u2013 Validation isn't enabled for the table in the migration task.</p> </li> <li> <p>Pending records \\u2013 Some records in the table are waiting for validation.</p> </li> <li> <p>Mismatched records \\u2013 Some records in the table don't match between the source and target.</p> </li> <li> <p>Suspended records \\u2013 Some records in the table couldn't be validated.</p> </li> <li> <p>No primary key \\u2013The table couldn't be validated because it has no primary key.</p> </li> <li> <p>Table error \\u2013 The table wasn't validated because it's in an error state and some data wasn't migrated.</p> </li> <li> <p>Validated \\u2013 All rows in the\
  \ table are validated. If the table is updated, the status can change from Validated.</p> </li> <li> <p>Error \\u2013 The table couldn't be validated because of an unexpected error.</p> </li> <li> <p>Pending validation \\u2013 The table is waiting validation.</p> </li> <li> <p>Preparing table \\u2013 Preparing the table enabled in the migration task for validation.</p> </li> <li> <p>Pending revalidation \\u2013 All rows in the table are pending validation after the table was updated.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ValidationStateDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Additional details about the state of validation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-table-statistics-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: TableStatistics
---
