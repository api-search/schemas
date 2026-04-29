---
description: Describes a directory that is used with Amazon WorkSpaces.
layout: schema
name: WorkspaceDirectory
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: Alias
  type: object
- description: ''
  name: DirectoryName
  type: object
- description: ''
  name: RegistrationCode
  type: object
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: DnsIpAddresses
  type: object
- description: ''
  name: CustomerUserName
  type: object
- description: ''
  name: IamRoleId
  type: object
- description: ''
  name: DirectoryType
  type: object
- description: ''
  name: WorkspaceSecurityGroupId
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: WorkspaceCreationProperties
  type: object
- description: ''
  name: ipGroupIds
  type: object
- description: ''
  name: WorkspaceAccessProperties
  type: object
- description: ''
  name: Tenancy
  type: object
- description: ''
  name: SelfservicePermissions
  type: object
- description: ''
  name: SamlProperties
  type: object
- description: ''
  name: CertificateBasedAuthProperties
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-workspace-directory-schema.json
slug: workspaces-workspace-directory
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier.\"\n        }\n      ]\n    },\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alias\"\n        },\n        {\n          \"description\": \"The directory alias.\"\n        }\n      ]\n    },\n    \"DirectoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryName\"\n        },\n        {\n          \"description\": \"The name of the directory.\"\n        }\n      ]\n    },\n    \"RegistrationCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationCode\"\n        },\n        {\n          \"description\": \"The registration code for the directory. This is the code that users enter in their Amazon WorkSpaces client application\
  \ to connect to the directory.\"\n        }\n      ]\n    },\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetIds\"\n        },\n        {\n          \"description\": \"The identifiers of the subnets used with the directory.\"\n        }\n      ]\n    },\n    \"DnsIpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsIpAddresses\"\n        },\n        {\n          \"description\": \"The IP addresses of the DNS servers for the directory.\"\n        }\n      ]\n    },\n    \"CustomerUserName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserName\"\n        },\n        {\n          \"description\": \"The user name for the service account.\"\n        }\n      ]\n    },\n    \"IamRoleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The identifier of the IAM role. This is the\
  \ role that allows Amazon WorkSpaces to make calls to other services, such as Amazon EC2, on your behalf.\"\n        }\n      ]\n    },\n    \"DirectoryType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceDirectoryType\"\n        },\n        {\n          \"description\": \"The directory type.\"\n        }\n      ]\n    },\n    \"WorkspaceSecurityGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupId\"\n        },\n        {\n          \"description\": \"The identifier of the security group that is assigned to new WorkSpaces.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceDirectoryState\"\n        },\n        {\n          \"description\": \"The state of the directory's registration with Amazon WorkSpaces. After a directory is deregistered, the <code>DEREGISTERED</code> state is returned very briefly before the directory\
  \ metadata is cleaned up, so this state is rarely returned. To confirm that a directory is deregistered, check for the directory ID by using <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/api/API_DescribeWorkspaceDirectories.html\\\"> DescribeWorkspaceDirectories</a>. If the directory ID isn't returned, then the directory has been successfully deregistered.\"\n        }\n      ]\n    },\n    \"WorkspaceCreationProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultWorkspaceCreationProperties\"\n        },\n        {\n          \"description\": \"The default creation properties for all WorkSpaces in the directory.\"\n        }\n      ]\n    },\n    \"ipGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpGroupIdList\"\n        },\n        {\n          \"description\": \"The identifiers of the IP access control groups associated with the directory.\"\n        }\n      ]\n    },\n    \"WorkspaceAccessProperties\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceAccessProperties\"\n        },\n        {\n          \"description\": \"The devices and operating systems that users can use to access WorkSpaces.\"\n        }\n      ]\n    },\n    \"Tenancy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tenancy\"\n        },\n        {\n          \"description\": \"Specifies whether the directory is dedicated or shared. To use Bring Your Own License (BYOL), this value must be set to <code>DEDICATED</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/workspaces/latest/adminguide/byol-windows-images.html\\\">Bring Your Own Windows Desktop Images</a>.\"\n        }\n      ]\n    },\n    \"SelfservicePermissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelfservicePermissions\"\n        },\n        {\n          \"description\": \"The default self-service permissions for WorkSpaces\
  \ in the directory.\"\n        }\n      ]\n    },\n    \"SamlProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SamlProperties\"\n        },\n        {\n          \"description\": \"Describes the enablement status, user access URL, and relay state parameter name that are used for configuring federation with an SAML 2.0 identity provider.\"\n        }\n      ]\n    },\n    \"CertificateBasedAuthProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateBasedAuthProperties\"\n        },\n        {\n          \"description\": \"The certificate-based authentication properties used to authenticate SAML 2.0 Identity Provider (IdP) user identities to Active Directory for WorkSpaces login.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes a directory that is used with Amazon WorkSpaces.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkspaceDirectory\",\n \
  \ \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-directory-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-workspace-directory-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: WorkspaceDirectory
---
