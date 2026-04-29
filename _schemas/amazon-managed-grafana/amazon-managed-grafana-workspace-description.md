---
description: A structure containing information about an Amazon Managed Grafana workspace in your account.
layout: schema
name: WorkspaceDescription
properties_list:
- description: ''
  name: accountAccessType
  type: object
- description: ''
  name: authentication
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: dataSources
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: endpoint
  type: object
- description: ''
  name: freeTrialConsumed
  type: object
- description: ''
  name: freeTrialExpiration
  type: object
- description: ''
  name: grafanaVersion
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: licenseExpiration
  type: object
- description: ''
  name: licenseType
  type: object
- description: ''
  name: modified
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: networkAccessControl
  type: object
- description: ''
  name: notificationDestinations
  type: object
- description: ''
  name: organizationRoleName
  type: object
- description: ''
  name: organizationalUnits
  type: object
- description: ''
  name: permissionType
  type: object
- description: ''
  name: stackSetName
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: vpcConfiguration
  type: object
- description: ''
  name: workspaceRoleArn
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-workspace-description-schema.json
slug: amazon-managed-grafana-workspace-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-workspace-description-schema.json\",\n  \"title\": \"WorkspaceDescription\",\n  \"description\": \"A structure containing information about an Amazon Managed Grafana workspace in your account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountAccessType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountAccessType\"\n        },\n        {\n          \"description\": \"Specifies whether the workspace can access Amazon Web Services resources in this Amazon Web Services account only, or whether it can also access Amazon Web Services resources in other accounts in the same organization. If this is <code>ORGANIZATION</code>, the <code>workspaceOrganizationalUnits</code> parameter specifies which organizational units the workspace\
  \ can access.\"\n        }\n      ]\n    },\n    \"authentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthenticationSummary\"\n        },\n        {\n          \"description\": \"A structure that describes whether the workspace uses SAML, IAM Identity Center, or both methods for user authentication.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date that the workspace was created.\"\n        }\n      ]\n    },\n    \"dataSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataSourceTypesList\"\n        },\n        {\n          \"description\": \"<p>Specifies the Amazon Web Services data sources that have been configured to have IAM roles and permissions created to allow Amazon Managed Grafana to read data from these sources.</p> <p>This list is only used when the\
  \ workspace was created through the Amazon Web Services console, and the <code>permissionType</code> is <code>SERVICE_MANAGED</code>.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The user-defined description of the workspace.\"\n        }\n      ]\n    },\n    \"endpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Endpoint\"\n        },\n        {\n          \"description\": \"The URL that users can use to access the Grafana console in the workspace.\"\n        }\n      ]\n    },\n    \"freeTrialConsumed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies whether this workspace has already fully used its free trial for Grafana Enterprise.\"\n        }\n      ]\n    },\n    \"freeTrialExpiration\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If this workspace is currently in the free trial period for Grafana Enterprise, this value specifies when that free trial ends.\"\n        }\n      ]\n    },\n    \"grafanaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrafanaVersion\"\n        },\n        {\n          \"description\": \"The version of Grafana supported in this workspace.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The unique ID of this workspace.\"\n        }\n      ]\n    },\n    \"licenseExpiration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"If this workspace has a full Grafana Enterprise license, this\
  \ specifies when the license ends and will need to be renewed.\"\n        }\n      ]\n    },\n    \"licenseType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LicenseType\"\n        },\n        {\n          \"description\": \"Specifies whether this workspace has a full Grafana Enterprise license or a free trial license.\"\n        }\n      ]\n    },\n    \"modified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The most recent date that the workspace was modified.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceName\"\n        },\n        {\n          \"description\": \"The name of the workspace.\"\n        }\n      ]\n    },\n    \"networkAccessControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkAccessConfiguration\"\n        },\n \
  \       {\n          \"description\": \"The configuration settings for network access to your workspace.\"\n        }\n      ]\n    },\n    \"notificationDestinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationDestinationsList\"\n        },\n        {\n          \"description\": \"The Amazon Web Services notification channels that Amazon Managed Grafana can automatically create IAM roles and permissions for, to allow Amazon Managed Grafana to use these channels.\"\n        }\n      ]\n    },\n    \"organizationRoleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationRoleName\"\n        },\n        {\n          \"description\": \"The name of the IAM role that is used to access resources through Organizations.\"\n        }\n      ]\n    },\n    \"organizationalUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationalUnitList\"\n        },\n        {\n  \
  \        \"description\": \"Specifies the organizational units that this workspace is allowed to use data sources from, if this workspace is in an account that is part of an organization.\"\n        }\n      ]\n    },\n    \"permissionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionType\"\n        },\n        {\n          \"description\": \"<p>If this is <code>SERVICE_MANAGED</code>, and the workplace was created through the Amazon Managed Grafana console, then Amazon Managed Grafana automatically creates the IAM roles and provisions the permissions that the workspace needs to use Amazon Web Services data sources and notification channels.</p> <p>If this is <code>CUSTOMER_MANAGED</code>, you must manage those roles and permissions yourself.</p> <p>If you are working with a workspace in a member account of an organization and that account is not a delegated administrator account, and you want the workspace to access data sources in other Amazon\
  \ Web Services accounts in the organization, this parameter must be set to <code>CUSTOMER_MANAGED</code>.</p> <p>For more information about converting between customer and service managed, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-datasource-and-notification.html\\\">Managing permissions for data sources and notification channels</a>. For more information about the roles and permissions that must be managed for customer managed workspaces, see <a href=\\\"https://docs.aws.amazon.com/grafana/latest/userguide/AMG-manage-permissions.html\\\">Amazon Managed Grafana permissions and policies for Amazon Web Services data sources and notification channels</a> </p>\"\n        }\n      ]\n    },\n    \"stackSetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StackSetName\"\n        },\n        {\n          \"description\": \"The name of the CloudFormation stack set that is used to generate IAM roles to be used for this workspace.\"\
  \n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceStatus\"\n        },\n        {\n          \"description\": \"The current status of the workspace.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of tags associated with the workspace.\"\n        }\n      ]\n    },\n    \"vpcConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcConfiguration\"\n        },\n        {\n          \"description\": \"The configuration for connecting to data sources in a private VPC (Amazon Virtual Private Cloud).\"\n        }\n      ]\n    },\n    \"workspaceRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IamRoleArn\"\n        },\n        {\n          \"description\": \"The IAM role that grants permissions\
  \ to the Amazon Web Services resources that the workspace will view data from. This role must already exist.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"authentication\",\n    \"created\",\n    \"dataSources\",\n    \"endpoint\",\n    \"grafanaVersion\",\n    \"id\",\n    \"modified\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-workspace-description-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: WorkspaceDescription
---
