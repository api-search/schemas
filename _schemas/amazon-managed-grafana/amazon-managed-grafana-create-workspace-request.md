---
description: CreateWorkspaceRequest schema from Amazon Managed Grafana API
layout: schema
name: CreateWorkspaceRequest
properties_list:
- description: ''
  name: accountAccessType
  type: object
- description: ''
  name: authenticationProviders
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: configuration
  type: object
- description: ''
  name: grafanaVersion
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
  name: stackSetName
  type: object
- description: ''
  name: tags
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
schema_file: json-schema/amazon-managed-grafana-create-workspace-request-schema.json
slug: amazon-managed-grafana-create-workspace-request
source_filename: amazon-managed-grafana-create-workspace-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-create-workspace-request-schema.json\",\n  \"title\": \"CreateWorkspaceRequest\",\n  \"description\": \"CreateWorkspaceRequest schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountAccessType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAccessType\"\n        },\n        {\n          \"description\": \"Specifies whether the workspace can access Amazon Web Services resources in this Amazon Web Services account only, or whether it can also access Amazon Web Services resources in other accounts in the same organization. If you specify <code>ORGANIZATION</code>, you must specify which organizational units the workspace can access in the <code>workspaceOrganizationalUnits</code> parameter.\"\
  \n        }\n      ]\n    },\n    \"authenticationProviders\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationProviders\"\n        },\n        {\n          \"description\": \"Specifies whether this workspace uses SAML 2.0, IAM Identity Center (successor to Single Sign-On), or both to authenticate users for using the Grafana console within a workspace. For more information, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/authentication-in-AMG.html\\\">User authentication in Amazon Managed Grafana</a>.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive, user-provided identifier to ensure the idempotency of the request.\"\n        }\n      ]\n    },\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OverridableConfigurationJson\"\
  \n        },\n        {\n          \"description\": \"The configuration string for the workspace that you create. For more information about the format and configuration options available, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-configure-workspace.html\\\">Working in your Grafana workspace</a>.\"\n        }\n      ]\n    },\n    \"grafanaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrafanaVersion\"\n        },\n        {\n          \"description\": \"<p>Specifies the version of Grafana to support in the new workspace.</p> <p>To get a list of supported version, use the <code>ListVersions</code> operation.</p>\"\n        }\n      ]\n    },\n    \"networkAccessControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkAccessConfiguration\"\n        },\n        {\n          \"description\": \"<p>Configuration for network access to your workspace.</p> <p>When this is configured,\
  \ only listed IP addresses and VPC endpoints will be able to access your workspace. Standard Grafana authentication and authorization will still be required.</p> <p>If this is not configured, or is removed, then all IP addresses and VPC endpoints will be allowed. Standard Grafana authentication and authorization will still be required.</p>\"\n        }\n      ]\n    },\n    \"organizationRoleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationRoleName\"\n        },\n        {\n          \"description\": \"The name of an IAM role that already exists to use with Organizations to access Amazon Web Services data sources and notification channels in other accounts in an organization.\"\n        }\n      ]\n    },\n    \"permissionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionType\"\n        },\n        {\n          \"description\": \"<p>When creating a workspace through the Amazon Web Services API,\
  \ CLI or Amazon Web Services CloudFormation, you must manage IAM roles and provision the permissions that the workspace needs to use Amazon Web Services data sources and notification channels.</p> <p>You must also specify a <code>workspaceRoleArn</code> for a role that you will manage for the workspace to use when accessing those datasources and notification channels.</p> <p>The ability for Amazon Managed Grafana to create and update IAM roles on behalf of the user is supported only in the Amazon Managed Grafana console, where this value may be set to <code>SERVICE_MANAGED</code>.</p> <note> <p>Use only the <code>CUSTOMER_MANAGED</code> permission type when creating a workspace with the API, CLI or Amazon Web Services CloudFormation. </p> </note> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-manage-permissions.html\\\">Amazon Managed Grafana permissions and policies for Amazon Web Services data sources and notification channels</a>.</p>\"\
  \n        }\n      ]\n    },\n    \"stackSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StackSetName\"\n        },\n        {\n          \"description\": \"The name of the CloudFormation stack set to use to generate IAM roles to be used for this workspace.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of tags associated with the workspace.\"\n        }\n      ]\n    },\n    \"vpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfiguration\"\n        },\n        {\n          \"description\": \"<p>The configuration settings for an Amazon VPC that contains data sources for your Grafana workspace to connect to.</p> <note> <p>Connecting to a private VPC is not yet available in the Asia Pacific (Seoul) Region (ap-northeast-2).</p> </note>\"\n        }\n    \
  \  ]\n    },\n    \"workspaceDataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceTypesList\"\n        },\n        {\n          \"description\": \"This parameter is for internal use only, and should not be used.\"\n        }\n      ]\n    },\n    \"workspaceDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"<p>A description for the workspace. This is used only to help you identify this workspace.</p> <p>Pattern: <code>^[\\\\\\\\p{L}\\\\\\\\p{Z}\\\\\\\\p{N}\\\\\\\\p{P}]{0,2048}$</code> </p>\"\n        }\n      ]\n    },\n    \"workspaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceName\"\n        },\n        {\n          \"description\": \"The name for the workspace. It does not have to be unique.\"\n        }\n      ]\n    },\n    \"workspaceNotificationDestinations\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/NotificationDestinationsList\"\n        },\n        {\n          \"description\": \"Specify the Amazon Web Services notification channels that you plan to use in this workspace. Specifying these data sources here enables Amazon Managed Grafana to create IAM roles and permissions that allow Amazon Managed Grafana to use these channels.\"\n        }\n      ]\n    },\n    \"workspaceOrganizationalUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationalUnitList\"\n        },\n        {\n          \"description\": \"Specifies the organizational units that this workspace is allowed to use data sources from, if this workspace is in an account that is part of an organization.\"\n        }\n      ]\n    },\n    \"workspaceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"Specified the IAM role\
  \ that grants permissions to the Amazon Web Services resources that the workspace will view data from, including both data sources and notification channels. You are responsible for managing the permissions for this role as new data sources or notification channels are added. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountAccessType\",\n    \"authenticationProviders\",\n    \"permissionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-create-workspace-request-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: CreateWorkspaceRequest
---
