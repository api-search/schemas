---
description: Describes the default properties that are used for creating WorkSpaces. For more information, see <a href="https://docs.aws.amazon.com/workspaces/latest/adminguide/update-directory-details.html">Update Directory Details for Your WorkSpaces</a>.
layout: schema
name: WorkspaceCreationProperties
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
schema_file: json-schema/workspaces-workspace-creation-properties-schema.json
slug: workspaces-workspace-creation-properties
source_filename: workspaces-workspace-creation-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"EnableWorkDocs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"<p>Indicates whether Amazon WorkDocs is enabled for your WorkSpaces.</p> <note> <p>If WorkDocs is already enabled for a WorkSpaces directory and you disable it, new WorkSpaces launched in the directory will not have WorkDocs enabled. However, WorkDocs remains enabled for any existing WorkSpaces, unless you either disable users' access to WorkDocs or you delete the WorkDocs site. To disable users' access to WorkDocs, see <a href=\\\"https://docs.aws.amazon.com/workdocs/latest/adminguide/inactive-user.html\\\">Disabling Users</a> in the <i>Amazon WorkDocs Administration Guide</i>. To delete a WorkDocs site, see <a href=\\\"https://docs.aws.amazon.com/workdocs/latest/adminguide/manage-sites.html\\\">Deleting a Site</a> in the <i>Amazon WorkDocs Administration Guide</i>.</p>\
  \ <p>If you enable WorkDocs on a directory that already has existing WorkSpaces, the existing WorkSpaces and any new WorkSpaces that are launched in the directory will have WorkDocs enabled.</p> </note>\"\n        }\n      ]\n    },\n    \"EnableInternetAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether internet access is enabled for your WorkSpaces.\"\n        }\n      ]\n    },\n    \"DefaultOu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultOu\"\n        },\n        {\n          \"description\": \"<p>The default organizational unit (OU) for your WorkSpaces directories. This string must be the full Lightweight Directory Access Protocol (LDAP) distinguished name for the target domain and OU. It must be in the form <code>\\\"OU=<i>value</i>,DC=<i>value</i>,DC=<i>value</i>\\\"</code>, where <i>value</i> is any string of characters,\
  \ and the number of domain components (DCs) is two or more. For example, <code>OU=WorkSpaces_machines,DC=machines,DC=example,DC=com</code>. </p> <important> <ul> <li> <p>To avoid errors, certain characters in the distinguished name must be escaped. For more information, see <a href=\\\"https://docs.microsoft.com/previous-versions/windows/desktop/ldap/distinguished-names\\\"> Distinguished Names</a> in the Microsoft documentation.</p> </li> <li> <p>The API doesn't validate whether the OU exists.</p> </li> </ul> </important>\"\n        }\n      ]\n    },\n    \"CustomSecurityGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupId\"\n        },\n        {\n          \"description\": \"The identifier of your custom security group.\"\n        }\n      ]\n    },\n    \"UserEnabledAsLocalAdministrator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\"\
  : \"Indicates whether users are local administrators of their WorkSpaces.\"\n        }\n      ]\n    },\n    \"EnableMaintenanceMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanObject\"\n        },\n        {\n          \"description\": \"Indicates whether maintenance mode is enabled for your WorkSpaces. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/workspace-maintenance.html\\\">WorkSpace Maintenance</a>. \"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the default properties that are used for creating WorkSpaces. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/update-directory-details.html\\\">Update Directory Details for Your WorkSpaces</a>. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceCreationProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-creation-properties-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-creation-properties-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceCreationProperties
---
