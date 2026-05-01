---
description: UpdateWorkspaceRequest schema from Amazon Managed Grafana API
layout: schema
name: UpdateWorkspaceRequest
properties_list:
- description: ''
  name: accountAccessType
  type: object
- description: ''
  name: networkAccessControl
  type: object
- description: ''
  name: organizationRoleName
  type: object
- description: ''
  name: permissionType
  type: object
- description: ''
  name: removeNetworkAccessConfiguration
  type: object
- description: ''
  name: removeVpcConfiguration
  type: object
- description: ''
  name: stackSetName
  type: object
- description: ''
  name: vpcConfiguration
  type: object
- description: ''
  name: workspaceDataSources
  type: object
- description: ''
  name: workspaceDescription
  type: object
- description: ''
  name: workspaceName
  type: object
- description: ''
  name: workspaceNotificationDestinations
  type: object
- description: ''
  name: workspaceOrganizationalUnits
  type: object
- description: ''
  name: workspaceRoleArn
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-update-workspace-request-schema.json
slug: amazon-managed-grafana-update-workspace-request
source_filename: amazon-managed-grafana-update-workspace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-workspace-request-schema.json\",\n  \"title\": \"UpdateWorkspaceRequest\",\n  \"description\": \"UpdateWorkspaceRequest schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountAccessType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAccessType\"\n        },\n        {\n          \"description\": \"Specifies whether the workspace can access Amazon Web Services resources in this Amazon Web Services account only, or whether it can also access Amazon Web Services resources in other accounts in the same organization. If you specify <code>ORGANIZATION</code>, you must specify which organizational units the workspace can access in the <code>workspaceOrganizationalUnits</code> parameter.\"\
  \n        }\n      ]\n    },\n    \"networkAccessControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkAccessConfiguration\"\n        },\n        {\n          \"description\": \"<p>The configuration settings for network access to your workspace.</p> <p>When this is configured, only listed IP addresses and VPC endpoints will be able to access your workspace. Standard Grafana authentication and authorization will still be required.</p> <p>If this is not configured, or is removed, then all IP addresses and VPC endpoints will be allowed. Standard Grafana authentication and authorization will still be required.</p>\"\n        }\n      ]\n    },\n    \"organizationRoleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationRoleName\"\n        },\n        {\n          \"description\": \"The name of an IAM role that already exists to use to access resources through Organizations. This can only be used with a workspace\
  \ that has the <code>permissionType</code> set to <code>CUSTOMER_MANAGED</code>.\"\n        }\n      ]\n    },\n    \"permissionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionType\"\n        },\n        {\n          \"description\": \"<p>Use this parameter if you want to change a workspace from <code>SERVICE_MANAGED</code> to <code>CUSTOMER_MANAGED</code>. This allows you to manage the permissions that the workspace uses to access datasources and notification channels. If the workspace is in a member Amazon Web Services account of an organization, and that account is not a delegated administrator account, and you want the workspace to access data sources in other Amazon Web Services accounts in the organization, you must choose <code>CUSTOMER_MANAGED</code>.</p> <p>If you specify this as <code>CUSTOMER_MANAGED</code>, you must also specify a <code>workspaceRoleArn</code> that the workspace will use for accessing Amazon Web Services resources.</p>\
  \ <p>For more information on the role and permissions needed, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-manage-permissions.html\\\">Amazon Managed Grafana permissions and policies for Amazon Web Services data sources and notification channels</a> </p> <note> <p>Do not use this to convert a <code>CUSTOMER_MANAGED</code> workspace to <code>SERVICE_MANAGED</code>. Do not include this parameter if you want to leave the workspace as <code>SERVICE_MANAGED</code>.</p> <p>You can convert a <code>CUSTOMER_MANAGED</code> workspace to <code>SERVICE_MANAGED</code> using the Amazon Managed Grafana console. For more information, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-datasource-and-notification.html\\\">Managing permissions for data sources and notification channels</a>.</p> </note>\"\n        }\n      ]\n    },\n    \"removeNetworkAccessConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\
  \n        },\n        {\n          \"description\": \"<p>Whether to remove the network access configuration from the workspace.</p> <p>Setting this to <code>true</code> and providing a <code>networkAccessControl</code> to set will return an error.</p> <p>If you remove this configuration by setting this to <code>true</code>, then all IP addresses and VPC endpoints will be allowed. Standard Grafana authentication and authorization will still be required.</p>\"\n        }\n      ]\n    },\n    \"removeVpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Whether to remove the VPC configuration from the workspace.</p> <p>Setting this to <code>true</code> and providing a <code>vpcConfiguration</code> to set will return an error.</p>\"\n        }\n      ]\n    },\n    \"stackSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StackSetName\"\n      \
  \  },\n        {\n          \"description\": \"The name of the CloudFormation stack set to use to generate IAM roles to be used for this workspace.\"\n        }\n      ]\n    },\n    \"vpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfiguration\"\n        },\n        {\n          \"description\": \"The configuration settings for an Amazon VPC that contains data sources for your Grafana workspace to connect to.\"\n        }\n      ]\n    },\n    \"workspaceDataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceTypesList\"\n        },\n        {\n          \"description\": \"This parameter is for internal use only, and should not be used.\"\n        }\n      ]\n    },\n    \"workspaceDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description for the workspace. This is used only\
  \ to help you identify this workspace.\"\n        }\n      ]\n    },\n    \"workspaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceName\"\n        },\n        {\n          \"description\": \"A new name for the workspace to update.\"\n        }\n      ]\n    },\n    \"workspaceNotificationDestinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationDestinationsList\"\n        },\n        {\n          \"description\": \"Specify the Amazon Web Services notification channels that you plan to use in this workspace. Specifying these data sources here enables Amazon Managed Grafana to create IAM roles and permissions that allow Amazon Managed Grafana to use these channels.\"\n        }\n      ]\n    },\n    \"workspaceOrganizationalUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationalUnitList\"\n        },\n        {\n          \"description\": \"Specifies\
  \ the organizational units that this workspace is allowed to use data sources from, if this workspace is in an account that is part of an organization.\"\n        }\n      ]\n    },\n    \"workspaceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"Specifies an IAM role that grants permissions to Amazon Web Services resources that the workspace accesses, such as data sources and notification channels. If this workspace has <code>permissionType</code> <code>CUSTOMER_MANAGED</code>, then this role is required.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-workspace-request-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: UpdateWorkspaceRequest
---
