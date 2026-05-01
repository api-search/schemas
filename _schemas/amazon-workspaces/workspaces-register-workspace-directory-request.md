---
description: RegisterWorkspaceDirectoryRequest schema from Amazon WorkSpaces API
layout: schema
name: RegisterWorkspaceDirectoryRequest
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: EnableWorkDocs
  type: object
- description: ''
  name: EnableSelfService
  type: object
- description: ''
  name: Tenancy
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-register-workspace-directory-request-schema.json
slug: workspaces-register-workspace-directory-request
source_filename: workspaces-register-workspace-directory-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"DirectoryId\",\n    \"EnableWorkDocs\"\n  ],\n  \"title\": \"RegisterWorkspaceDirectoryRequest\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory. You cannot register a directory if it does not have a status of Active. If the directory does not have a status of Active, you will receive an InvalidResourceStateException error. If you have already registered the maximum number of directories that you can register with Amazon WorkSpaces, you will receive a ResourceLimitExceededException error. Deregister directories that you are not using for WorkSpaces, and try again.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"\
  The identifiers of the subnets for your virtual private cloud (VPC). Make sure that the subnets are in supported Availability Zones. The subnets must also be in separate Availability Zones. If these conditions are not met, you will receive an OperationNotSupportedException error.\"\n        }\n      ]\n    },\n    \"EnableWorkDocs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether Amazon WorkDocs is enabled or disabled. If you have enabled this parameter and WorkDocs is not available in the Region, you will receive an OperationNotSupportedException error. Set <code>EnableWorkDocs</code> to disabled, and try again.\"\n        }\n      ]\n    },\n    \"EnableSelfService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether self-service capabilities are enabled or\
  \ disabled.\"\n        }\n      ]\n    },\n    \"Tenancy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tenancy\"\n        },\n        {\n          \"description\": \"Indicates whether your WorkSpace directory is dedicated or shared. To use Bring Your Own License (BYOL) images, this value must be set to <code>DEDICATED</code> and your Amazon Web Services account must be enabled for BYOL. If your account has not been enabled for BYOL, you will receive an InvalidParameterValuesException error. For more information about BYOL images, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/byol-windows-images.html\\\">Bring Your Own Windows Desktop Images</a>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags associated with the directory.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-register-workspace-directory-request-schema.json\",\n  \"description\": \"RegisterWorkspaceDirectoryRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-register-workspace-directory-request-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: RegisterWorkspaceDirectoryRequest
---
