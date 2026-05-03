---
description: An entity (table) definition in a relational data model, including its attributes, primary key, and relationships to other entities.
layout: schema
name: Relational Data Model Entity
properties_list:
- description: The name of the entity/table.
  name: name
  type: string
- description: Description of the entity and its purpose.
  name: description
  type: string
- description: Database schema the entity belongs to.
  name: schema
  type: string
- description: List of attributes (columns) in the entity.
  name: attributes
  type: array
- description: List of attribute names forming the primary key.
  name: primaryKey
  type: array
- description: Foreign key relationships to other entities.
  name: foreignKeys
  type: array
- description: Additional indexes on the entity.
  name: indexes
  type: array
- description: The highest normal form this entity satisfies.
  name: normalForm
  type: string
provider_name: Relational Data Modeling
provider_slug: relational-data-modeling
schema_file: json-schema/relational-data-modeling-entity-schema.json
slug: relational-data-modeling-entity
source_filename: relational-data-modeling-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/relational-data-modeling/main/json-schema/relational-data-modeling-entity-schema.json\",\n  \"title\": \"Relational Data Model Entity\",\n  \"description\": \"An entity (table) definition in a relational data model, including its attributes, primary key, and relationships to other entities.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"attributes\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity/table.\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the entity and its purpose.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Database schema the entity belongs to.\"\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"List\
  \ of attributes (columns) in the entity.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Attribute\"\n      },\n      \"minItems\": 1\n    },\n    \"primaryKey\": {\n      \"type\": \"array\",\n      \"description\": \"List of attribute names forming the primary key.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1\n    },\n    \"foreignKeys\": {\n      \"type\": \"array\",\n      \"description\": \"Foreign key relationships to other entities.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ForeignKey\"\n      }\n    },\n    \"indexes\": {\n      \"type\": \"array\",\n      \"description\": \"Additional indexes on the entity.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Index\"\n      }\n    },\n    \"normalForm\": {\n      \"type\": \"string\",\n      \"description\": \"The highest normal form this entity satisfies.\",\n      \"enum\": [\"1NF\", \"2NF\", \"3NF\", \"BCNF\", \"4NF\", \"5NF\"]\n    }\n  },\n  \"$defs\": {\n    \"Attribute\"\
  : {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"dataType\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The attribute/column name.\"\n        },\n        \"dataType\": {\n          \"type\": \"string\",\n          \"description\": \"SQL data type (e.g., VARCHAR, INTEGER, BOOLEAN, DATE).\"\n        },\n        \"nullable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the attribute can be NULL.\",\n          \"default\": true\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the attribute must be unique.\",\n          \"default\": false\n        },\n        \"default\": {\n          \"description\": \"Default value for the attribute.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the attribute.\"\n        },\n        \"isPrimaryKey\": {\n        \
  \  \"type\": \"boolean\",\n          \"description\": \"Whether this attribute is part of the primary key.\",\n          \"default\": false\n        }\n      }\n    },\n    \"ForeignKey\": {\n      \"type\": \"object\",\n      \"required\": [\"columns\", \"referencedEntity\", \"referencedColumns\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the foreign key constraint.\"\n        },\n        \"columns\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Columns in this entity forming the foreign key.\"\n        },\n        \"referencedEntity\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the referenced entity.\"\n        },\n        \"referencedColumns\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Columns in the referenced entity.\"\n        },\n        \"\
  onDelete\": {\n          \"type\": \"string\",\n          \"enum\": [\"CASCADE\", \"SET NULL\", \"RESTRICT\", \"NO ACTION\"],\n          \"description\": \"Action on delete.\"\n        },\n        \"onUpdate\": {\n          \"type\": \"string\",\n          \"enum\": [\"CASCADE\", \"SET NULL\", \"RESTRICT\", \"NO ACTION\"],\n          \"description\": \"Action on update.\"\n        }\n      }\n    },\n    \"Index\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"columns\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the index.\"\n        },\n        \"columns\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Columns included in the index.\"\n        },\n        \"unique\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the index enforces uniqueness.\",\n          \"default\": false\n        },\n        \"\
  type\": {\n          \"type\": \"string\",\n          \"enum\": [\"BTREE\", \"HASH\", \"GIN\", \"GIST\", \"BRIN\"],\n          \"description\": \"Index implementation type.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/relational-data-modeling/refs/heads/main/json-schema/relational-data-modeling-entity-schema.json
tags:
- Data Architecture
- Database Design
- Entity Relationship
- Normalization
- SQL
- Schema Design
- Data Modeling
title: Relational Data Model Entity
---
