---
description: Describes the default values that are used to create WorkSpaces. For more information, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/update-directory-details.html">Update Directory Details for Your WorkSpaces</a>.
layout: schema
name: DefaultWorkspaceCreationProperties
properties_list:
- description: ''
  name: EnableWorkDocs
  type: object
- description: ''
  name: EnableInternetAccess
  type: object
- description: ''
  name: DefaultOu
  type: object
- description: ''
  name: CustomSecurityGroupId
  type: object
- description: ''
  name: UserEnabledAsLocalAdministrator
  type: object
- description: ''
  name: EnableMaintenanceMode
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-default-workspace-creation-properties-schema.json
slug: workspaces-default-workspace-creation-properties
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EnableWorkDocs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Specifies whether the directory is enabled for Amazon WorkDocs.\"\n        }\n      ]\n    },\n    \"EnableInternetAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Specifies whether to automatically assign an Elastic public IP address to WorkSpaces in this directory by default. If enabled, the Elastic public IP address allows outbound internet access from your WorkSpaces when you\\u2019re using an internet gateway in the Amazon VPC in which your WorkSpaces are located. If you're using a Network Address Translation (NAT) gateway for outbound internet access from your VPC, or if your WorkSpaces are in public subnets and you manually assign them Elastic IP\
  \ addresses, you should disable this setting. This setting applies to new WorkSpaces that you launch or to existing WorkSpaces that you rebuild. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/amazon-workspaces-vpc.html\\\"> Configure a VPC for Amazon WorkSpaces</a>.\"\n        }\n      ]\n    },\n    \"DefaultOu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultOu\"\n        },\n        {\n          \"description\": \"The organizational unit (OU) in the directory for the WorkSpace machine accounts.\"\n        }\n      ]\n    },\n    \"CustomSecurityGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the default security group to apply to WorkSpaces when they are created. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/amazon-workspaces-security-groups.html\\\
  \"> Security Groups for Your WorkSpaces</a>.\"\n        }\n      ]\n    },\n    \"UserEnabledAsLocalAdministrator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Specifies whether WorkSpace users are local administrators on their WorkSpaces.\"\n        }\n      ]\n    },\n    \"EnableMaintenanceMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Specifies whether maintenance mode is enabled for WorkSpaces. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/workspace-maintenance.html\\\">WorkSpace Maintenance</a>.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the default values that are used to create WorkSpaces. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/update-directory-details.html\\\
  \">Update Directory Details for Your WorkSpaces</a>.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DefaultWorkspaceCreationProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-default-workspace-creation-properties-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-default-workspace-creation-properties-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DefaultWorkspaceCreationProperties
---
