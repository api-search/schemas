---
description: ConnectorEntityField schema from Amazon AppFlow API
layout: schema
name: ConnectorEntityField
properties_list:
- description: The unique identifier of the connector field.
  name: identifier
  type: string
- description: The parent identifier of the connector field.
  name: parentIdentifier
  type: string
- description: The label applied to a connector entity field.
  name: label
  type: string
- description: Booelan value that indicates whether this field can be used as a primary key.
  name: isPrimaryKey
  type: boolean
- description: Default value that can be assigned to this field.
  name: defaultValue
  type: string
- description: Booelan value that indicates whether this field is deprecated or not.
  name: isDeprecated
  type: boolean
- description: Contains details regarding the supported FieldType, including the corresponding filterOperators and supportedValues.
  name: supportedFieldTypeDetails
  type: object
- description: A description of the connector entity field.
  name: description
  type: string
- description: The properties that can be applied to a field when the connector is being used as a source.
  name: sourceProperties
  type: object
- description: The properties applied to a field when the connector is being used as a destination.
  name: destinationProperties
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-connector-entity-field-schema.json
slug: appflow-connector-entity-field
source_filename: appflow-connector-entity-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-entity-field-schema.json\",\n  \"title\": \"ConnectorEntityField\",\n  \"description\": \"ConnectorEntityField schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"type\": \"string\",\n      \"example\": \"Id\",\n      \"description\": \"The unique identifier of the connector field.\"\n    },\n    \"parentIdentifier\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The parent identifier of the connector field.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Account ID\",\n      \"description\": \"The label applied to a connector entity field.\"\n    },\n    \"isPrimaryKey\": {\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"description\": \"Booelan\
  \ value that indicates whether this field can be used as a primary key.\"\n    },\n    \"defaultValue\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"Default value that can be assigned to this field.\"\n    },\n    \"isDeprecated\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Booelan value that indicates whether this field is deprecated or not.\"\n    },\n    \"supportedFieldTypeDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Contains details regarding the supported FieldType, including the corresponding filterOperators and supportedValues.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"The unique identifier for the Account object.\",\n      \"description\": \"A description of the connector entity field.\"\n    },\n    \"sourceProperties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isQueryable\": {\n          \"type\": \"boolean\"\
  ,\n          \"example\": true\n        },\n        \"isRetrievable\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isPartitioningSupported\": {\n          \"type\": \"boolean\",\n          \"example\": false\n        }\n      },\n      \"description\": \"The properties that can be applied to a field when the connector is being used as a source.\"\n    },\n    \"destinationProperties\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isCreatable\": {\n          \"type\": \"boolean\",\n          \"example\": false\n        },\n        \"isNullable\": {\n          \"type\": \"boolean\",\n          \"example\": false\n        },\n        \"isUpsertable\": {\n          \"type\": \"boolean\",\n          \"example\": false\n        },\n        \"isUpdatable\": {\n          \"type\": \"boolean\",\n          \"example\": false\n        },\n        \"isDefaultedOnCreate\": {\n          \"type\": \"boolean\",\n          \"example\": false\n\
  \        },\n        \"supportedWriteOperations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"example\": \"\"\n          },\n          \"example\": [\n            \"INSERT\"\n          ]\n        }\n      },\n      \"description\": \"The properties applied to a field when the connector is being used as a destination.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-entity-field-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ConnectorEntityField
---
