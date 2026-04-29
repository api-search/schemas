---
description: Information about one or more IP address blocks.
layout: schema
name: IpRouteInfo
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: CidrIp
  type: object
- description: ''
  name: IpRouteStatusMsg
  type: object
- description: ''
  name: AddedDateTime
  type: object
- description: ''
  name: IpRouteStatusReason
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-ip-route-info-schema.json
slug: amazon-directory-service-ip-route-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-ip-route-info-schema.json\",\n  \"title\": \"IpRouteInfo\",\n  \"description\": \"Information about one or more IP address blocks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"Identifier (ID) of the directory associated with the IP addresses.\"\n        }\n      ]\n    },\n    \"CidrIp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CidrIp\"\n        },\n        {\n          \"description\": \"IP address block in the <a>IpRoute</a>.\"\n        }\n      ]\n    },\n    \"IpRouteStatusMsg\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRouteStatusMsg\"\
  \n        },\n        {\n          \"description\": \"The status of the IP address block.\"\n        }\n      ]\n    },\n    \"AddedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddedDateTime\"\n        },\n        {\n          \"description\": \"The date and time the address block was added to the directory.\"\n        }\n      ]\n    },\n    \"IpRouteStatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpRouteStatusReason\"\n        },\n        {\n          \"description\": \"The reason for the IpRouteStatusMsg.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"Description of the <a>IpRouteInfo</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-ip-route-info-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: IpRouteInfo
---
