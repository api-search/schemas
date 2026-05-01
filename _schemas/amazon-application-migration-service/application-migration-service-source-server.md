---
description: A source server registered with the Application Migration Service
layout: schema
name: SourceServer
properties_list:
- description: Unique identifier for the source server
  name: sourceServerID
  type: string
- description: ARN of the source server
  name: arn
  type: string
- description: Whether the source server is archived
  name: isArchived
  type: boolean
- description: Tags applied to the source server
  name: tags
  type: object
- description: lifeCycle
  name: lifeCycle
  type: string
- description: dataReplicationInfo
  name: dataReplicationInfo
  type: string
- description: sourceProperties
  name: sourceProperties
  type: string
- description: launchedInstance
  name: launchedInstance
  type: string
- description: ID of the application this server belongs to
  name: applicationID
  type: string
- description: ID of the vCenter client this server was discovered from
  name: vcenterClientID
  type: string
- description: Replication type for the source server
  name: replicationType
  type: string
- description: User-provided identifier for the source server
  name: userProvidedID
  type: string
- description: FQDN used for action framework connectivity
  name: fqdnForActionFramework
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-source-server-schema.json
slug: application-migration-service-source-server
source_filename: application-migration-service-source-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-source-server-schema.json\",\n  \"title\": \"SourceServer\",\n  \"description\": \"A source server registered with the Application Migration Service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the source server\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the source server\"\n    },\n    \"isArchived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the source server is archived\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags applied to the source server\"\n    },\n    \"lifeCycle\": {\n      \"type\": \"string\",\n      \"description\": \"lifeCycle\"\n    },\n    \"dataReplicationInfo\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"dataReplicationInfo\"\n    },\n    \"sourceProperties\": {\n      \"type\": \"string\",\n      \"description\": \"sourceProperties\"\n    },\n    \"launchedInstance\": {\n      \"type\": \"string\",\n      \"description\": \"launchedInstance\"\n    },\n    \"applicationID\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the application this server belongs to\"\n    },\n    \"vcenterClientID\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the vCenter client this server was discovered from\"\n    },\n    \"replicationType\": {\n      \"type\": \"string\",\n      \"description\": \"Replication type for the source server\"\n    },\n    \"userProvidedID\": {\n      \"type\": \"string\",\n      \"description\": \"User-provided identifier for the source server\"\n    },\n    \"fqdnForActionFramework\": {\n      \"type\": \"string\",\n      \"description\": \"FQDN used for action framework connectivity\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-source-server-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: SourceServer
---
