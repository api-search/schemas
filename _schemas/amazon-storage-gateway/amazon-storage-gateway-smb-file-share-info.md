---
description: The Windows file permissions and ownership information assigned, by default, to native S3 objects when S3 File Gateway discovers them in S3 buckets. This operation is only supported for S3 File Gateways.
layout: schema
name: SMBFileShareInfo
properties_list:
- description: ''
  name: FileShareARN
  type: object
- description: ''
  name: FileShareId
  type: object
- description: ''
  name: FileShareStatus
  type: object
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: KMSEncrypted
  type: object
- description: ''
  name: KMSKey
  type: object
- description: ''
  name: Path
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: LocationARN
  type: object
- description: ''
  name: DefaultStorageClass
  type: object
- description: ''
  name: ObjectACL
  type: object
- description: ''
  name: ReadOnly
  type: object
- description: ''
  name: GuessMIMETypeEnabled
  type: object
- description: ''
  name: RequesterPays
  type: object
- description: ''
  name: SMBACLEnabled
  type: object
- description: ''
  name: AccessBasedEnumeration
  type: object
- description: ''
  name: AdminUserList
  type: object
- description: ''
  name: ValidUserList
  type: object
- description: ''
  name: InvalidUserList
  type: object
- description: ''
  name: AuditDestinationARN
  type: object
- description: ''
  name: Authentication
  type: object
- description: ''
  name: CaseSensitivity
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: FileShareName
  type: object
- description: ''
  name: CacheAttributes
  type: object
- description: ''
  name: NotificationPolicy
  type: object
- description: ''
  name: VPCEndpointDNSName
  type: object
- description: ''
  name: BucketRegion
  type: object
- description: ''
  name: OplocksEnabled
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-smb-file-share-info-schema.json
slug: amazon-storage-gateway-smb-file-share-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-smb-file-share-info-schema.json\",\n  \"title\": \"SMBFileShareInfo\",\n  \"description\": \"The Windows file permissions and ownership information assigned, by default, to native S3 objects when S3 File Gateway discovers them in S3 buckets. This operation is only supported for S3 File Gateways.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileShareARN\": {\n      \"$ref\": \"#/components/schemas/FileShareARN\"\n    },\n    \"FileShareId\": {\n      \"$ref\": \"#/components/schemas/FileShareId\"\n    },\n    \"FileShareStatus\": {\n      \"$ref\": \"#/components/schemas/FileShareStatus\"\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"KMSEncrypted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\
  \n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to use Amazon S3 server-side encryption with your own KMS key, or <code>false</code> to use a key managed by Amazon S3. Optional.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"KMSKey\": {\n      \"$ref\": \"#/components/schemas/KMSKey\"\n    },\n    \"Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Path\"\n        },\n        {\n          \"description\": \"The file share path used by the SMB client to identify the mount point.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"$ref\": \"#/components/schemas/Role\"\n    },\n    \"LocationARN\": {\n      \"$ref\": \"#/components/schemas/LocationARN\"\n    },\n    \"DefaultStorageClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageClass\"\n        },\n        {\n          \"description\": \"<p>The default storage class for\
  \ objects put into an Amazon S3 bucket by the S3 File Gateway. The default value is <code>S3_STANDARD</code>. Optional.</p> <p>Valid Values: <code>S3_STANDARD</code> | <code>S3_INTELLIGENT_TIERING</code> | <code>S3_STANDARD_IA</code> | <code>S3_ONEZONE_IA</code> </p>\"\n        }\n      ]\n    },\n    \"ObjectACL\": {\n      \"$ref\": \"#/components/schemas/ObjectACL\"\n    },\n    \"ReadOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A value that sets the write status of a file share. Set this value to <code>true</code> to set the write status to read-only, otherwise set to <code>false</code>.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"GuessMIMETypeEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A value that enables guessing\
  \ of the MIME type for uploaded objects based on file extensions. Set this value to <code>true</code> to enable MIME type guessing, otherwise set to <code>false</code>. The default value is <code>true</code>.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"RequesterPays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A value that sets who pays the cost of the request and the cost associated with data download from the S3 bucket. If this value is set to <code>true</code>, the requester pays the costs; otherwise, the S3 bucket owner pays. However, the S3 bucket owner always pays the cost of storing data.</p> <note> <p> <code>RequesterPays</code> is a configuration for the S3 bucket that backs the file share, so make sure that the configuration on the file share is the same as the S3 bucket configuration.</p> </note> <p>Valid Values: <code>true</code>\
  \ | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"SMBACLEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>If this value is set to <code>true</code>, it indicates that access control list (ACL) is enabled on the SMB file share. If it is set to <code>false</code>, it indicates that file and directory permissions are mapped to the POSIX permission.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/storagegateway/latest/userguide/smb-acl.html\\\">Using Microsoft Windows ACLs to control access to an SMB file share</a> in the <i>Storage Gateway User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"AccessBasedEnumeration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether <code>AccessBasedEnumeration</code> is enabled.\"\n        }\n      ]\n\
  \    },\n    \"AdminUserList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"A list of users or groups in the Active Directory that have administrator rights to the file share. A group must be prefixed with the @ character. Acceptable formats include: <code>DOMAIN\\\\User1</code>, <code>user1</code>, <code>@group1</code>, and <code>@DOMAIN\\\\group1</code>. Can only be set if Authentication is set to <code>ActiveDirectory</code>.\"\n        }\n      ]\n    },\n    \"ValidUserList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"A list of users or groups in the Active Directory that are allowed to access the file share. A group must be prefixed with the @ character. Acceptable formats include: <code>DOMAIN\\\\User1</code>, <code>user1</code>, <code>@group1</code>, and <code>@DOMAIN\\\\group1</code>.\
  \ Can only be set if Authentication is set to <code>ActiveDirectory</code>.\"\n        }\n      ]\n    },\n    \"InvalidUserList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"A list of users or groups in the Active Directory that are not allowed to access the file share. A group must be prefixed with the @ character. Acceptable formats include: <code>DOMAIN\\\\User1</code>, <code>user1</code>, <code>@group1</code>, and <code>@DOMAIN\\\\group1</code>. Can only be set if Authentication is set to <code>ActiveDirectory</code>.\"\n        }\n      ]\n    },\n    \"AuditDestinationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditDestinationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the storage used for audit logs.\"\n        }\n      ]\n    },\n    \"Authentication\": {\n      \"$ref\": \"#/components/schemas/Authentication\"\
  \n    },\n    \"CaseSensitivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaseSensitivity\"\n        },\n        {\n          \"description\": \"The case of an object name in an Amazon S3 bucket. For <code>ClientSpecified</code>, the client determines the case sensitivity. For <code>CaseSensitive</code>, the gateway determines the case sensitivity. The default value is <code>ClientSpecified</code>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"A list of up to 50 tags assigned to the SMB file share, sorted alphabetically by key name. Each tag is a key-value pair. For a gateway with more than 10 tags assigned, you can view all tags using the <code>ListTagsForResource</code> API operation.\"\n        }\n      ]\n    },\n    \"FileShareName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareName\"\
  \n        },\n        {\n          \"description\": \"<p>The name of the file share. Optional.</p> <note> <p> <code>FileShareName</code> must be set if an S3 prefix name is set in <code>LocationARN</code>, or if an access point or access point alias is used.</p> </note>\"\n        }\n      ]\n    },\n    \"CacheAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CacheAttributes\"\n        },\n        {\n          \"description\": \"Refresh cache information for the file share.\"\n        }\n      ]\n    },\n    \"NotificationPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotificationPolicy\"\n        },\n        {\n          \"description\": \"<p>The notification policy of the file share. <code>SettlingTimeInSeconds</code> controls the number of seconds to wait after the last point in time a client wrote to a file before generating an <code>ObjectUploaded</code> notification. Because clients can make many small\
  \ writes to files, it's best to set this parameter for as long as possible to avoid generating multiple notifications for the same file in a small time period.</p> <note> <p> <code>SettlingTimeInSeconds</code> has no effect on the timing of the object uploading to Amazon S3, only the timing of the notification.</p> </note> <p>The following example sets <code>NotificationPolicy</code> on with <code>SettlingTimeInSeconds</code> set to 60.</p> <p> <code>{\\\\\\\"Upload\\\\\\\": {\\\\\\\"SettlingTimeInSeconds\\\\\\\": 60}}</code> </p> <p>The following example sets <code>NotificationPolicy</code> off.</p> <p> <code>{}</code> </p>\"\n        }\n      ]\n    },\n    \"VPCEndpointDNSName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DNSHostName\"\n        },\n        {\n          \"description\": \"<p>Specifies the DNS name for the VPC endpoint that the SMB file share uses to connect to Amazon S3.</p> <note> <p>This parameter is required for SMB file shares that\
  \ connect to Amazon S3 through a VPC endpoint, a VPC access point, or an access point alias that points to a VPC access point.</p> </note>\"\n        }\n      ]\n    },\n    \"BucketRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionId\"\n        },\n        {\n          \"description\": \"<p>Specifies the Region of the S3 bucket where the SMB file share stores files.</p> <note> <p>This parameter is required for SMB file shares that connect to Amazon S3 through a VPC endpoint, a VPC access point, or an access point alias that points to a VPC access point.</p> </note>\"\n        }\n      ]\n    },\n    \"OplocksEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Specifies whether opportunistic locking is enabled for the SMB file share.</p> <note> <p>Enabling opportunistic locking on case-sensitive shares is not recommended for workloads that involve\
  \ access to files with the same name in different case.</p> </note> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-smb-file-share-info-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: SMBFileShareInfo
---
