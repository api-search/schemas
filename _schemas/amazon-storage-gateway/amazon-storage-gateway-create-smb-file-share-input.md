---
description: CreateSMBFileShareInput
layout: schema
name: CreateSMBFileShareInput
properties_list:
- description: ''
  name: ClientToken
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
schema_file: json-schema/amazon-storage-gateway-create-smb-file-share-input-schema.json
slug: amazon-storage-gateway-create-smb-file-share-input
source_filename: amazon-storage-gateway-create-smb-file-share-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-smb-file-share-input-schema.json\",\n  \"title\": \"CreateSMBFileShareInput\",\n  \"description\": \"CreateSMBFileShareInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A unique string value that you supply that is used by S3 File Gateway to ensure idempotent file share creation.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The ARN of the S3 File Gateway on which you want to create a file share.\"\n        }\n      ]\n    },\n    \"KMSEncrypted\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Set to <code>true</code> to use Amazon S3 server-side encryption with your own KMS key, or <code>false</code> to use a key managed by Amazon S3. Optional.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"KMSKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KMSKey\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a symmetric customer master key (CMK) used for Amazon S3 server-side encryption. Storage Gateway does not support asymmetric CMKs. This value can only be set when <code>KMSEncrypted</code> is <code>true</code>. Optional.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The ARN of the Identity\
  \ and Access Management (IAM) role that an S3 File Gateway assumes when it accesses the underlying storage.\"\n        }\n      ]\n    },\n    \"LocationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationARN\"\n        },\n        {\n          \"description\": \"<p>A custom ARN for the backend storage used for storing data for file shares. It includes a resource ARN with an optional prefix concatenation. The prefix must end with a forward slash (/).</p> <note> <p>You can specify LocationARN as a bucket ARN, access point ARN or access point alias, as shown in the following examples.</p> <p>Bucket ARN:</p> <p> <code>arn:aws:s3:::my-bucket/prefix/</code> </p> <p>Access point ARN:</p> <p> <code>arn:aws:s3:region:account-id:accesspoint/access-point-name/prefix/</code> </p> <p>If you specify an access point, the bucket policy must be configured to delegate access control to the access point. For information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-points-policies.html#access-points-delegating-control\\\
  \">Delegating access control to access points</a> in the <i>Amazon S3 User Guide</i>.</p> <p>Access point alias:</p> <p> <code>test-ap-ab123cdef4gehijklmn5opqrstuvuse1a-s3alias</code> </p> </note>\"\n        }\n      ]\n    },\n    \"DefaultStorageClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageClass\"\n        },\n        {\n          \"description\": \"<p>The default storage class for objects put into an Amazon S3 bucket by the S3 File Gateway. The default value is <code>S3_STANDARD</code>. Optional.</p> <p>Valid Values: <code>S3_STANDARD</code> | <code>S3_INTELLIGENT_TIERING</code> | <code>S3_STANDARD_IA</code> | <code>S3_ONEZONE_IA</code> </p>\"\n        }\n      ]\n    },\n    \"ObjectACL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ObjectACL\"\n        },\n        {\n          \"description\": \"A value that sets the access control list (ACL) permission for objects in the S3 bucket that a S3 File Gateway\
  \ puts objects into. The default value is <code>private</code>.\"\n        }\n      ]\n    },\n    \"ReadOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A value that sets the write status of a file share. Set this value to <code>true</code> to set the write status to read-only, otherwise set to <code>false</code>.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"GuessMIMETypeEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A value that enables guessing of the MIME type for uploaded objects based on file extensions. Set this value to <code>true</code> to enable MIME type guessing, otherwise set to <code>false</code>. The default value is <code>true</code>.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n      \
  \  }\n      ]\n    },\n    \"RequesterPays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>A value that sets who pays the cost of the request and the cost associated with data download from the S3 bucket. If this value is set to <code>true</code>, the requester pays the costs; otherwise, the S3 bucket owner pays. However, the S3 bucket owner always pays the cost of storing data.</p> <note> <p> <code>RequesterPays</code> is a configuration for the S3 bucket that backs the file share, so make sure that the configuration on the file share is the same as the S3 bucket configuration.</p> </note> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"SMBACLEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Set this value to <code>true</code> to enable\
  \ access control list (ACL) on the SMB file share. Set it to <code>false</code> to map file and directory permissions to the POSIX permissions.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/storagegateway/latest/userguide/smb-acl.html\\\">Using Microsoft Windows ACLs to control access to an SMB file share</a> in the <i>Storage Gateway User Guide</i>.</p> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    },\n    \"AccessBasedEnumeration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The files and folders on this share will only be visible to users with read access.\"\n        }\n      ]\n    },\n    \"AdminUserList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"<p>A list of users or groups in the Active Directory that will be granted\
  \ administrator privileges on the file share. These users can do all file operations as the super-user. Acceptable formats include: <code>DOMAIN\\\\User1</code>, <code>user1</code>, <code>@group1</code>, and <code>@DOMAIN\\\\group1</code>.</p> <important> <p>Use this option very carefully, because any user in this list can do anything they like on the file share, regardless of file permissions.</p> </important>\"\n        }\n      ]\n    },\n    \"ValidUserList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"A list of users or groups in the Active Directory that are allowed to access the file <a href=\\\"\\\"/> share. A group must be prefixed with the @ character. Acceptable formats include: <code>DOMAIN\\\\User1</code>, <code>user1</code>, <code>@group1</code>, and <code>@DOMAIN\\\\group1</code>. Can only be set if Authentication is set to <code>ActiveDirectory</code>.\"\n        }\n      ]\n\
  \    },\n    \"InvalidUserList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserList\"\n        },\n        {\n          \"description\": \"A list of users or groups in the Active Directory that are not allowed to access the file share. A group must be prefixed with the @ character. Acceptable formats include: <code>DOMAIN\\\\User1</code>, <code>user1</code>, <code>@group1</code>, and <code>@DOMAIN\\\\group1</code>. Can only be set if Authentication is set to <code>ActiveDirectory</code>.\"\n        }\n      ]\n    },\n    \"AuditDestinationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditDestinationARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the storage used for audit logs.\"\n        }\n      ]\n    },\n    \"Authentication\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Authentication\"\n        },\n        {\n          \"description\"\
  : \"<p>The authentication method that users use to access the file share. The default is <code>ActiveDirectory</code>.</p> <p>Valid Values: <code>ActiveDirectory</code> | <code>GuestAccess</code> </p>\"\n        }\n      ]\n    },\n    \"CaseSensitivity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CaseSensitivity\"\n        },\n        {\n          \"description\": \"The case of an object name in an Amazon S3 bucket. For <code>ClientSpecified</code>, the client determines the case sensitivity. For <code>CaseSensitive</code>, the gateway determines the case sensitivity. The default value is <code>ClientSpecified</code>.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"<p>A list of up to 50 tags that can be assigned to the NFS file share. Each tag is a key-value pair.</p> <note> <p>Valid characters for key and value are letters,\
  \ spaces, and numbers representable in UTF-8 format, and the following special characters: + - = . _ : / @. The maximum length of a tag's key is 128 characters, and the maximum length for a tag's value is 256.</p> </note>\"\n        }\n      ]\n    },\n    \"FileShareName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareName\"\n        },\n        {\n          \"description\": \"<p>The name of the file share. Optional.</p> <note> <p> <code>FileShareName</code> must be set if an S3 prefix name is set in <code>LocationARN</code>, or if an access point or access point alias is used.</p> </note>\"\n        }\n      ]\n    },\n    \"CacheAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CacheAttributes\"\n        },\n        {\n          \"description\": \"Specifies refresh cache information for the file share.\"\n        }\n      ]\n    },\n    \"NotificationPolicy\": {\n      \"allOf\": [\n        {\n       \
  \   \"$ref\": \"#/components/schemas/NotificationPolicy\"\n        },\n        {\n          \"description\": \"<p>The notification policy of the file share. <code>SettlingTimeInSeconds</code> controls the number of seconds to wait after the last point in time a client wrote to a file before generating an <code>ObjectUploaded</code> notification. Because clients can make many small writes to files, it's best to set this parameter for as long as possible to avoid generating multiple notifications for the same file in a small time period.</p> <note> <p> <code>SettlingTimeInSeconds</code> has no effect on the timing of the object uploading to Amazon S3, only the timing of the notification.</p> </note> <p>The following example sets <code>NotificationPolicy</code> on with <code>SettlingTimeInSeconds</code> set to 60.</p> <p> <code>{\\\\\\\"Upload\\\\\\\": {\\\\\\\"SettlingTimeInSeconds\\\\\\\": 60}}</code> </p> <p>The following example sets <code>NotificationPolicy</code> off.</p> <p> <code>{}</code>\
  \ </p>\"\n        }\n      ]\n    },\n    \"VPCEndpointDNSName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DNSHostName\"\n        },\n        {\n          \"description\": \"<p>Specifies the DNS name for the VPC endpoint that the SMB file share uses to connect to Amazon S3.</p> <note> <p>This parameter is required for SMB file shares that connect to Amazon S3 through a VPC endpoint, a VPC access point, or an access point alias that points to a VPC access point.</p> </note>\"\n        }\n      ]\n    },\n    \"BucketRegion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionId\"\n        },\n        {\n          \"description\": \"<p>Specifies the Region of the S3 bucket where the SMB file share stores files.</p> <note> <p>This parameter is required for SMB file shares that connect to Amazon S3 through a VPC endpoint, a VPC access point, or an access point alias that points to a VPC access point.</p> </note>\"\n     \
  \   }\n      ]\n    },\n    \"OplocksEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Specifies whether opportunistic locking is enabled for the SMB file share.</p> <note> <p>Enabling opportunistic locking on case-sensitive shares is not recommended for workloads that involve access to files with the same name in different case.</p> </note> <p>Valid Values: <code>true</code> | <code>false</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClientToken\",\n    \"GatewayARN\",\n    \"Role\",\n    \"LocationARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-smb-file-share-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateSMBFileShareInput
---
