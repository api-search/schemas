---
description: Details about the shared directory in the directory owner account for which the share request in the directory consumer account has been accepted.
layout: schema
name: SharedDirectory
properties_list:
- description: ''
  name: OwnerAccountId
  type: object
- description: ''
  name: OwnerDirectoryId
  type: object
- description: ''
  name: ShareMethod
  type: object
- description: ''
  name: SharedAccountId
  type: object
- description: ''
  name: SharedDirectoryId
  type: object
- description: ''
  name: ShareStatus
  type: object
- description: ''
  name: ShareNotes
  type: object
- description: ''
  name: CreatedDateTime
  type: object
- description: ''
  name: LastUpdatedDateTime
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-shared-directory-schema.json
slug: amazon-directory-service-shared-directory
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-shared-directory-schema.json\",\n  \"title\": \"SharedDirectory\",\n  \"description\": \"Details about the shared directory in the directory owner account for which the share request in the directory consumer account has been accepted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OwnerAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"Identifier of the directory owner account, which contains the directory that has been shared to the consumer account.\"\n        }\n      ]\n    },\n    \"OwnerDirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"Identifier\
  \ of the directory in the directory owner account. \"\n        }\n      ]\n    },\n    \"ShareMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareMethod\"\n        },\n        {\n          \"description\": \"The method used when sharing a directory to determine whether the directory should be shared within your Amazon Web Services organization (<code>ORGANIZATIONS</code>) or with any Amazon Web Services account by sending a shared directory request (<code>HANDSHAKE</code>).\"\n        }\n      ]\n    },\n    \"SharedAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomerId\"\n        },\n        {\n          \"description\": \"Identifier of the directory consumer account that has access to the shared directory (<code>OwnerDirectoryId</code>) in the directory owner account.\"\n        }\n      ]\n    },\n    \"SharedDirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\
  \n        },\n        {\n          \"description\": \"Identifier of the shared directory in the directory consumer account. This identifier is different for each directory owner account.\"\n        }\n      ]\n    },\n    \"ShareStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareStatus\"\n        },\n        {\n          \"description\": \"Current directory status of the shared Managed Microsoft AD directory.\"\n        }\n      ]\n    },\n    \"ShareNotes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notes\"\n        },\n        {\n          \"description\": \"A directory share request that is sent by the directory owner to the directory consumer. The request includes a typed message to help the directory consumer administrator determine whether to approve or reject the share invitation.\"\n        }\n      ]\n    },\n    \"CreatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedDateTime\"\
  \n        },\n        {\n          \"description\": \"The date and time that the shared directory was created.\"\n        }\n      ]\n    },\n    \"LastUpdatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the shared directory was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-shared-directory-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: SharedDirectory
---
