---
description: Contains information about an Directory Service directory.
layout: schema
name: DirectoryDescription
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: ShortName
  type: object
- description: ''
  name: Size
  type: object
- description: ''
  name: Edition
  type: object
- description: ''
  name: Alias
  type: object
- description: ''
  name: AccessUrl
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: DnsIpAddrs
  type: object
- description: ''
  name: Stage
  type: object
- description: ''
  name: ShareStatus
  type: object
- description: ''
  name: ShareMethod
  type: object
- description: ''
  name: ShareNotes
  type: object
- description: ''
  name: LaunchTime
  type: object
- description: ''
  name: StageLastUpdatedDateTime
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: VpcSettings
  type: object
- description: ''
  name: ConnectSettings
  type: object
- description: ''
  name: RadiusSettings
  type: object
- description: ''
  name: RadiusStatus
  type: object
- description: ''
  name: StageReason
  type: object
- description: ''
  name: SsoEnabled
  type: object
- description: ''
  name: DesiredNumberOfDomainControllers
  type: object
- description: ''
  name: OwnerDirectoryDescription
  type: object
- description: ''
  name: RegionsInfo
  type: object
- description: ''
  name: OsVersion
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-directory-description-schema.json
slug: amazon-directory-service-directory-description
source_filename: amazon-directory-service-directory-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-description-schema.json\",\n  \"title\": \"DirectoryDescription\",\n  \"description\": \"Contains information about an Directory Service directory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryName\"\n        },\n        {\n          \"description\": \"The fully qualified name of the directory.\"\n        }\n      ]\n    },\n    \"ShortName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryShortName\"\
  \n        },\n        {\n          \"description\": \"The short name of the directory.\"\n        }\n      ]\n    },\n    \"Size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectorySize\"\n        },\n        {\n          \"description\": \"The directory size.\"\n        }\n      ]\n    },\n    \"Edition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryEdition\"\n        },\n        {\n          \"description\": \"The edition associated with this directory.\"\n        }\n      ]\n    },\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasName\"\n        },\n        {\n          \"description\": \"The alias for the directory. If no alias has been created for the directory, the alias is the directory identifier, such as <code>d-XXXXXXXXXX</code>.\"\n        }\n      ]\n    },\n    \"AccessUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessUrl\"\
  \n        },\n        {\n          \"description\": \"The access URL for the directory, such as <code>http://&lt;alias&gt;.awsapps.com</code>. If no alias has been created for the directory, <code>&lt;alias&gt;</code> is the directory identifier, such as <code>d-XXXXXXXXXX</code>.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description for the directory.\"\n        }\n      ]\n    },\n    \"DnsIpAddrs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DnsIpAddrs\"\n        },\n        {\n          \"description\": \"The IP addresses of the DNS servers for the directory. For a Simple AD or Microsoft AD directory, these are the IP addresses of the Simple AD or Microsoft AD directory servers. For an AD Connector directory, these are the IP addresses of the DNS servers or domain controllers in your self-managed\
  \ directory to which the AD Connector is connected.\"\n        }\n      ]\n    },\n    \"Stage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryStage\"\n        },\n        {\n          \"description\": \"The current stage of the directory.\"\n        }\n      ]\n    },\n    \"ShareStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareStatus\"\n        },\n        {\n          \"description\": \"Current directory status of the shared Managed Microsoft AD directory.\"\n        }\n      ]\n    },\n    \"ShareMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShareMethod\"\n        },\n        {\n          \"description\": \"The method used when sharing a directory to determine whether the directory should be shared within your Amazon Web Services organization (<code>ORGANIZATIONS</code>) or with any Amazon Web Services account by sending a shared directory request (<code>HANDSHAKE</code>).\"\
  \n        }\n      ]\n    },\n    \"ShareNotes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notes\"\n        },\n        {\n          \"description\": \"A directory share request that is sent by the directory owner to the directory consumer. The request includes a typed message to help the directory consumer administrator determine whether to approve or reject the share invitation.\"\n        }\n      ]\n    },\n    \"LaunchTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTime\"\n        },\n        {\n          \"description\": \"Specifies when the directory was created.\"\n        }\n      ]\n    },\n    \"StageLastUpdatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the stage was last updated.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/DirectoryType\"\n        },\n        {\n          \"description\": \"The directory size.\"\n        }\n      ]\n    },\n    \"VpcSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryVpcSettingsDescription\"\n        },\n        {\n          \"description\": \"A <a>DirectoryVpcSettingsDescription</a> object that contains additional information about a directory. This member is only present if the directory is a Simple AD or Managed Microsoft AD directory.\"\n        }\n      ]\n    },\n    \"ConnectSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryConnectSettingsDescription\"\n        },\n        {\n          \"description\": \"A <a>DirectoryConnectSettingsDescription</a> object that contains additional information about an AD Connector directory. This member is only present if the directory is an AD Connector directory.\"\n        }\n      ]\n   \
  \ },\n    \"RadiusSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusSettings\"\n        },\n        {\n          \"description\": \"A <a>RadiusSettings</a> object that contains information about the RADIUS server configured for this directory.\"\n        }\n      ]\n    },\n    \"RadiusStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RadiusStatus\"\n        },\n        {\n          \"description\": \"The status of the RADIUS MFA server connection.\"\n        }\n      ]\n    },\n    \"StageReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageReason\"\n        },\n        {\n          \"description\": \"Additional information about the directory stage.\"\n        }\n      ]\n    },\n    \"SsoEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SsoEnabled\"\n        },\n        {\n          \"description\": \"Indicates if single sign-on\
  \ is enabled for the directory. For more information, see <a>EnableSso</a> and <a>DisableSso</a>.\"\n        }\n      ]\n    },\n    \"DesiredNumberOfDomainControllers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredNumberOfDomainControllers\"\n        },\n        {\n          \"description\": \"The desired number of domain controllers in the directory if the directory is Microsoft AD.\"\n        }\n      ]\n    },\n    \"OwnerDirectoryDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerDirectoryDescription\"\n        },\n        {\n          \"description\": \"Describes the Managed Microsoft AD directory in the directory owner account.\"\n        }\n      ]\n    },\n    \"RegionsInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionsInfo\"\n        },\n        {\n          \"description\": \"Lists the Regions where the directory has replicated.\"\n        }\n      ]\n\
  \    },\n    \"OsVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OSVersion\"\n        },\n        {\n          \"description\": \"The operating system (OS) version of the directory.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-description-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: DirectoryDescription
---
