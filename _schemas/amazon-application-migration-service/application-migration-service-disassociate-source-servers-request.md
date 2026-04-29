---
description: Request to disassociate source servers from an application
layout: schema
name: DisassociateSourceServersRequest
properties_list:
- description: Application ID
  name: applicationID
  type: string
- description: Source server IDs to disassociate
  name: sourceServerIDs
  type: array
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-disassociate-source-servers-request-schema.json
slug: application-migration-service-disassociate-source-servers-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-disassociate-source-servers-request-schema.json\",\n  \"title\": \"DisassociateSourceServersRequest\",\n  \"description\": \"Request to disassociate source servers from an application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationID\": {\n      \"type\": \"string\",\n      \"description\": \"Application ID\"\n    },\n    \"sourceServerIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Source server IDs to disassociate\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-disassociate-source-servers-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DisassociateSourceServersRequest
---
