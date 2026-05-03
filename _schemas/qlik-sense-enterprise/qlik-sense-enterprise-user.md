---
description: A Qlik Sense user represents an identity imported from an external user directory (such as Active Directory or LDAP) into the Qlik Sense repository. Users are associated with user directories, can be assigned roles, and have their access controlled by security and license rules.
layout: schema
name: Qlik Sense User
properties_list:
- description: Unique identifier (GUID) assigned by the repository
  name: id
  type: string
- description: ISO 8601 timestamp when the user was created in the repository
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the user was last modified
  name: modifiedDate
  type: string
- description: Username of the user who last modified this record
  name: modifiedByUserName
  type: string
- description: Display name of the user
  name: name
  type: string
- description: Name of the user directory the user was imported from (e.g., Active Directory domain name)
  name: userDirectory
  type: string
- description: Unique user identifier within the user directory (e.g., sAMAccountName)
  name: userId
  type: string
- description: Roles assigned to the user, used in security and license rule evaluation
  name: roles
  type: array
- description: Whether the user account is inactive
  name: inactive
  type: boolean
- description: Whether the user has been removed from the external user directory
  name: removedExternally
  type: boolean
- description: Whether the user is blacklisted from accessing Qlik Sense
  name: blacklisted
  type: boolean
- description: Whether deletion of this user is prohibited (e.g., system accounts)
  name: deleteProhibited
  type: boolean
- description: Tags applied to the user for categorization
  name: tags
  type: array
- description: Custom property values assigned to the user
  name: customProperties
  type: array
- description: List of privileges the current user has on this user entity
  name: privileges
  type: array
- description: Schema path identifying the entity type in the QRS
  name: schemaPath
  type: string
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
schema_file: json-schema/qlik-sense-enterprise-user-schema.json
slug: qlik-sense-enterprise-user
source_filename: qlik-sense-enterprise-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.api.dev/qlik-sense-enterprise/user.json\",\n  \"title\": \"Qlik Sense User\",\n  \"description\": \"A Qlik Sense user represents an identity imported from an external user directory (such as Active Directory or LDAP) into the Qlik Sense repository. Users are associated with user directories, can be assigned roles, and have their access controlled by security and license rules.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier (GUID) assigned by the repository\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the user was created in the repository\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"\
  ISO 8601 timestamp when the user was last modified\"\n    },\n    \"modifiedByUserName\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the user who last modified this record\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the user\"\n    },\n    \"userDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the user directory the user was imported from (e.g., Active Directory domain name)\",\n      \"minLength\": 1\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique user identifier within the user directory (e.g., sAMAccountName)\",\n      \"minLength\": 1\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Roles assigned to the user, used in security and license rule evaluation\"\n    },\n    \"inactive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the user account is inactive\",\n      \"default\": false\n    },\n    \"removedExternally\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has been removed from the external user directory\",\n      \"default\": false\n    },\n    \"blacklisted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is blacklisted from accessing Qlik Sense\",\n      \"default\": false\n    },\n    \"deleteProhibited\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether deletion of this user is prohibited (e.g., system accounts)\",\n      \"default\": false\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TagReference\"\n      },\n      \"description\": \"Tags applied to the user for categorization\"\n    },\n    \"customProperties\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomPropertyValue\"\n      },\n      \"description\": \"Custom property\
  \ values assigned to the user\"\n    },\n    \"privileges\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of privileges the current user has on this user entity\"\n    },\n    \"schemaPath\": {\n      \"type\": \"string\",\n      \"description\": \"Schema path identifying the entity type in the QRS\"\n    }\n  },\n  \"required\": [\"userId\", \"userDirectory\"],\n  \"$defs\": {\n    \"TagReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"privileges\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"CustomPropertyValue\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n     \
  \     \"format\": \"uuid\"\n        },\n        \"definition\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"valueType\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"value\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/json-schema/qlik-sense-enterprise-user-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
title: Qlik Sense User
---
