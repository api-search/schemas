---
description: Schema for a Google Cloud Storage bucket resource as returned by the Cloud Storage JSON API v1. A bucket is a container for objects stored in Cloud Storage. Buckets are associated with a project, have globally unique names, and provide configuration for storage class, location, access control, lifecycle management, versioning, and encryption.
layout: schema
name: Google Cloud Storage Bucket
properties_list:
- description: The kind of item this is. For buckets, this is always storage#bucket.
  name: kind
  type: string
- description: The ID of the bucket. For buckets, this is the same value as the name property. Read-only.
  name: id
  type: string
- description: The URI of this bucket. Read-only.
  name: selfLink
  type: string
- description: The project number of the project the bucket belongs to. Read-only.
  name: projectNumber
  type: string
- description: The name of the bucket. Bucket names must be globally unique across all of Cloud Storage, contain only lowercase letters, numbers, hyphens, underscores, and dots, and must be between 3 and 63 characte
  name: name
  type: string
- description: The creation time of the bucket in RFC 3339 format. Read-only.
  name: timeCreated
  type: string
- description: The modification time of the bucket metadata in RFC 3339 format. Read-only.
  name: updated
  type: string
- description: The metadata generation of this bucket. Used for preconditions and for detecting changes in metadata. Every update to the bucket's metadata increments this value. Read-only.
  name: metageneration
  type: string
- description: 'The location of the bucket. Object data for objects in the bucket resides in physical storage within this region. Can be a multi-region (e.g., US, EU, ASIA), dual-region (e.g., US-EAST1+US-WEST1), or '
  name: location
  type: string
- description: The type of location that the bucket resides in. Read-only.
  name: locationType
  type: string
- description: The default storage class of the bucket, used for newly created objects when no storage class is specified. Objects can be stored in Standard, Nearline, Coldline, or Archive storage.
  name: storageClass
  type: string
- description: HTTP 1.1 Entity tag for the bucket. Read-only.
  name: etag
  type: string
- description: Whether or not to automatically apply an event-based hold to new objects added to the bucket. Event-based holds remain on an object until explicitly removed.
  name: defaultEventBasedHold
  type: boolean
- description: The Recovery Point Objective (RPO) of this bucket. Set to ASYNC_TURBO to enable Turbo Replication on dual-region buckets, providing a lower RPO of 15 minutes instead of the default.
  name: rpo
  type: string
- description: Access controls on the bucket, containing one or more bucketAccessControls resources. Not returned in list responses unless projection=full is specified.
  name: acl
  type:
  - array
  - 'null'
- description: Default access controls to apply to new objects when no ACL is provided.
  name: defaultObjectAcl
  type:
  - array
  - 'null'
- description: ''
  name: iamConfiguration
  type: object
- description: Encryption configuration for the bucket. Specifies a default Cloud KMS key for encrypting objects inserted into this bucket.
  name: encryption
  type:
  - object
  - 'null'
- description: The bucket's lifecycle configuration. Lifecycle management lets you set a Time to Live (TTL) for objects, or automatically transition objects to different storage classes based on conditions.
  name: lifecycle
  type:
  - object
  - 'null'
- description: The bucket's logging configuration, which defines the destination bucket and optional name prefix for the current bucket's access logs.
  name: logging
  type:
  - object
  - 'null'
- description: The bucket's versioning configuration. When enabled, Cloud Storage retains a noncurrent object version each time a live object version is replaced or deleted.
  name: versioning
  type:
  - object
  - 'null'
- description: The bucket's website configuration, controlling how the service behaves when accessing bucket contents as a web site.
  name: website
  type:
  - object
  - 'null'
- description: The bucket's Cross-Origin Resource Sharing (CORS) configuration to support requests from web applications running in browsers.
  name: cors
  type:
  - array
  - 'null'
- description: The bucket's retention policy, which defines the minimum age an object in the bucket must reach before it can be deleted or replaced.
  name: retentionPolicy
  type:
  - object
  - 'null'
- description: The bucket's soft delete policy. When enabled, deleted objects are retained for a specified period and can be recovered.
  name: softDeletePolicy
  type:
  - object
  - 'null'
- description: The bucket's Autoclass configuration. When enabled, Autoclass automatically transitions objects in the bucket to appropriate storage classes based on each object's access pattern.
  name: autoclass
  type:
  - object
  - 'null'
- description: The bucket's hierarchical namespace configuration. When enabled, the bucket supports folders and managed folders as organizational structures.
  name: hierarchicalNamespace
  type:
  - object
  - 'null'
- description: User-provided labels, in key/value pairs. Labels are used to organize and filter buckets. Keys and values must be 63 characters or less and conform to RFC 1035.
  name: labels
  type:
  - object
  - 'null'
- description: The bucket's custom placement configuration for Custom Dual Regions.
  name: customPlacementConfig
  type:
  - object
  - 'null'
- description: Whether the bucket satisfies zone separation requirements. Read-only.
  name: satisfiesPZS
  type: boolean
provider_name: Google Cloud Storage
provider_slug: gcp-cloud-storage
schema_file: json-schema/gcp-cloud-storage-bucket-schema.json
slug: gcp-cloud-storage-bucket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/storage/docs/json_api/v1/buckets\",\n  \"title\": \"Google Cloud Storage Bucket\",\n  \"description\": \"Schema for a Google Cloud Storage bucket resource as returned by the Cloud Storage JSON API v1. A bucket is a container for objects stored in Cloud Storage. Buckets are associated with a project, have globally unique names, and provide configuration for storage class, location, access control, lifecycle management, versioning, and encryption.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"storage#bucket\",\n      \"description\": \"The kind of item this is. For buckets, this is always storage#bucket.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the bucket. For buckets, this is the same value as the name property. Read-only.\"\
  ,\n      \"examples\": [\"my-bucket\", \"example-project-data\"]\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URI of this bucket. Read-only.\",\n      \"examples\": [\"https://storage.googleapis.com/storage/v1/b/my-bucket\"]\n    },\n    \"projectNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The project number of the project the bucket belongs to. Read-only.\",\n      \"examples\": [\"123456789012\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket. Bucket names must be globally unique across all of Cloud Storage, contain only lowercase letters, numbers, hyphens, underscores, and dots, and must be between 3 and 63 characters long.\",\n      \"minLength\": 3,\n      \"maxLength\": 63,\n      \"pattern\": \"^[a-z0-9][a-z0-9._-]{1,61}[a-z0-9]$\",\n      \"examples\": [\"my-bucket\", \"example-project-data\", \"company.backups.2024\"]\n    },\n \
  \   \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the bucket in RFC 3339 format. Read-only.\",\n      \"examples\": [\"2024-01-15T09:00:00.000Z\"]\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The modification time of the bucket metadata in RFC 3339 format. Read-only.\",\n      \"examples\": [\"2024-06-20T14:30:00.000Z\"]\n    },\n    \"metageneration\": {\n      \"type\": \"string\",\n      \"description\": \"The metadata generation of this bucket. Used for preconditions and for detecting changes in metadata. Every update to the bucket's metadata increments this value. Read-only.\",\n      \"examples\": [\"1\", \"5\"]\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the bucket. Object data for objects in the bucket resides in physical storage within this region. Can be a multi-region\
  \ (e.g., US, EU, ASIA), dual-region (e.g., US-EAST1+US-WEST1), or single region (e.g., US-EAST1).\",\n      \"examples\": [\"US\", \"US-EAST1\", \"EUROPE-WEST1\", \"ASIA-SOUTHEAST1\"]\n    },\n    \"locationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of location that the bucket resides in. Read-only.\",\n      \"enum\": [\"multi-region\", \"region\", \"dual-region\"]\n    },\n    \"storageClass\": {\n      \"type\": \"string\",\n      \"description\": \"The default storage class of the bucket, used for newly created objects when no storage class is specified. Objects can be stored in Standard, Nearline, Coldline, or Archive storage.\",\n      \"enum\": [\"STANDARD\", \"NEARLINE\", \"COLDLINE\", \"ARCHIVE\"],\n      \"examples\": [\"STANDARD\"]\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"description\": \"HTTP 1.1 Entity tag for the bucket. Read-only.\"\n    },\n    \"defaultEventBasedHold\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether or not to automatically apply an event-based hold to new objects added to the bucket. Event-based holds remain on an object until explicitly removed.\",\n      \"default\": false\n    },\n    \"rpo\": {\n      \"type\": \"string\",\n      \"description\": \"The Recovery Point Objective (RPO) of this bucket. Set to ASYNC_TURBO to enable Turbo Replication on dual-region buckets, providing a lower RPO of 15 minutes instead of the default.\",\n      \"enum\": [\"DEFAULT\", \"ASYNC_TURBO\"]\n    },\n    \"acl\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"Access controls on the bucket, containing one or more bucketAccessControls resources. Not returned in list responses unless projection=full is specified.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/BucketAccessControl\"\n      }\n    },\n    \"defaultObjectAcl\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"Default access controls to apply to new objects when no ACL is provided.\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/ObjectAccessControl\"\n      }\n    },\n    \"iamConfiguration\": {\n      \"$ref\": \"#/$defs/IamConfiguration\"\n    },\n    \"encryption\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Encryption configuration for the bucket. Specifies a default Cloud KMS key for encrypting objects inserted into this bucket.\",\n      \"properties\": {\n        \"defaultKmsKeyName\": {\n          \"type\": \"string\",\n          \"description\": \"A Cloud KMS key resource name that will be used to encrypt objects inserted into this bucket if no encryption method is specified. The key must be in the same location as the bucket.\",\n          \"examples\": [\"projects/my-project/locations/us/keyRings/my-keyring/cryptoKeys/my-key\"]\n        }\n      }\n    },\n    \"lifecycle\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's lifecycle configuration. Lifecycle management lets you set a Time to\
  \ Live (TTL) for objects, or automatically transition objects to different storage classes based on conditions.\",\n      \"properties\": {\n        \"rule\": {\n          \"type\": \"array\",\n          \"description\": \"A lifecycle management rule, consisting of an action and the condition(s) under which the action will be taken.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/LifecycleRule\"\n          }\n        }\n      }\n    },\n    \"logging\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's logging configuration, which defines the destination bucket and optional name prefix for the current bucket's access logs.\",\n      \"properties\": {\n        \"logBucket\": {\n          \"type\": \"string\",\n          \"description\": \"The destination bucket where the current bucket's access logs are placed.\"\n        },\n        \"logObjectPrefix\": {\n          \"type\": \"string\",\n          \"description\": \"A prefix for log object names.\
  \ Defaults to the name of the source bucket.\"\n        }\n      }\n    },\n    \"versioning\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's versioning configuration. When enabled, Cloud Storage retains a noncurrent object version each time a live object version is replaced or deleted.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether object versioning is fully enabled for the bucket.\"\n        }\n      }\n    },\n    \"website\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's website configuration, controlling how the service behaves when accessing bucket contents as a web site.\",\n      \"properties\": {\n        \"mainPageSuffix\": {\n          \"type\": \"string\",\n          \"description\": \"If the requested object path is missing, the service ensures the path has a trailing / and then appends this suffix. This allows the creation of\
  \ index.html objects to represent directory pages.\",\n          \"examples\": [\"index.html\"]\n        },\n        \"notFoundPage\": {\n          \"type\": \"string\",\n          \"description\": \"If the requested object path is missing and any mainPageSuffix object is missing, the service returns the named object from this bucket as the content for a 404 Not Found result.\",\n          \"examples\": [\"404.html\"]\n        }\n      }\n    },\n    \"cors\": {\n      \"type\": [\"array\", \"null\"],\n      \"description\": \"The bucket's Cross-Origin Resource Sharing (CORS) configuration to support requests from web applications running in browsers.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CorsConfiguration\"\n      }\n    },\n    \"retentionPolicy\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's retention policy, which defines the minimum age an object in the bucket must reach before it can be deleted or replaced.\",\n      \"properties\"\
  : {\n        \"retentionPeriod\": {\n          \"type\": \"string\",\n          \"description\": \"The duration in seconds that objects need to be retained. Retention duration must be greater than zero and less than 100 years (3,155,760,000 seconds).\",\n          \"examples\": [\"86400\", \"2592000\"]\n        },\n        \"effectiveTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The earliest date and time that the policy was effective. Read-only.\"\n        },\n        \"isLocked\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether or not the retention policy is locked. A locked retention policy cannot be removed or the retention period shortened. Read-only once locked.\"\n        }\n      }\n    },\n    \"softDeletePolicy\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's soft delete policy. When enabled, deleted objects are retained for a specified period and can\
  \ be recovered.\",\n      \"properties\": {\n        \"retentionDurationSeconds\": {\n          \"type\": \"string\",\n          \"description\": \"The number of seconds that soft-deleted objects will be retained and recoverable. Must be at least 604800 (7 days) and at most 7776000 (90 days).\",\n          \"examples\": [\"604800\", \"2592000\"]\n        },\n        \"effectiveTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The time from which the soft delete policy is or will be effective. Read-only.\"\n        }\n      }\n    },\n    \"autoclass\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's Autoclass configuration. When enabled, Autoclass automatically transitions objects in the bucket to appropriate storage classes based on each object's access pattern.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether Autoclass\
  \ is enabled for this bucket.\"\n        },\n        \"toggleTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The time at which Autoclass was last enabled or disabled for the bucket. Read-only.\"\n        },\n        \"terminalStorageClass\": {\n          \"type\": \"string\",\n          \"description\": \"The storage class that objects in the bucket eventually transition to if they are not read for a certain length of time. Valid values are NEARLINE and ARCHIVE.\",\n          \"enum\": [\"NEARLINE\", \"ARCHIVE\"]\n        },\n        \"terminalStorageClassUpdateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The time at which the terminal storage class was last updated. Read-only.\"\n        }\n      }\n    },\n    \"hierarchicalNamespace\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's hierarchical namespace configuration. When\
  \ enabled, the bucket supports folders and managed folders as organizational structures.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether hierarchical namespace is enabled for the bucket.\"\n        }\n      }\n    },\n    \"labels\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"User-provided labels, in key/value pairs. Labels are used to organize and filter buckets. Keys and values must be 63 characters or less and conform to RFC 1035.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        {\n          \"environment\": \"production\",\n          \"team\": \"data-engineering\"\n        }\n      ]\n    },\n    \"customPlacementConfig\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"The bucket's custom placement configuration for Custom Dual Regions.\",\n      \"properties\": {\n        \"dataLocations\": {\n    \
  \      \"type\": \"array\",\n          \"description\": \"The list of regional locations in which data is placed.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"minItems\": 2,\n          \"maxItems\": 2,\n          \"examples\": [[\"US-EAST1\", \"US-WEST1\"]]\n        }\n      }\n    },\n    \"satisfiesPZS\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the bucket satisfies zone separation requirements. Read-only.\"\n    }\n  },\n  \"additionalProperties\": true,\n  \"$defs\": {\n    \"BucketAccessControl\": {\n      \"type\": \"object\",\n      \"description\": \"An access-control entry for a bucket.\",\n      \"required\": [\"entity\", \"role\"],\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"const\": \"storage#bucketAccessControl\",\n          \"description\": \"The kind of item this is.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"The ID of the access-control entry.\"\n        },\n        \"selfLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The link to this access-control entry.\"\n        },\n        \"bucket\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the bucket.\"\n        },\n        \"entity\": {\n          \"type\": \"string\",\n          \"description\": \"The entity holding the permission, in one of the following forms: user-userId, user-email, group-groupId, group-email, domain-domain, project-team-projectId, allUsers, or allAuthenticatedUsers.\",\n          \"examples\": [\"user-example@gmail.com\", \"group-admins@example.com\", \"allUsers\"]\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"The access permission for the entity.\",\n          \"enum\": [\"OWNER\", \"WRITER\", \"READER\"]\n        },\n        \"email\": {\n          \"type\": [\"string\", \"null\"\
  ],\n          \"format\": \"email\",\n          \"description\": \"The email address associated with the entity, if any.\"\n        },\n        \"domain\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The domain associated with the entity, if any.\"\n        },\n        \"entityId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID for the entity, if any.\"\n        },\n        \"etag\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP 1.1 Entity tag for the access-control entry.\"\n        },\n        \"projectTeam\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"The project team associated with the entity, if any.\",\n          \"properties\": {\n            \"projectNumber\": {\n              \"type\": \"string\",\n              \"description\": \"The project number.\"\n            },\n            \"team\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"The team.\",\n              \"enum\": [\"editors\", \"owners\", \"viewers\"]\n            }\n          }\n        }\n      }\n    },\n    \"ObjectAccessControl\": {\n      \"type\": \"object\",\n      \"description\": \"An access-control entry for an object or default object ACL on a bucket.\",\n      \"required\": [\"entity\", \"role\"],\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"const\": \"storage#objectAccessControl\",\n          \"description\": \"The kind of item this is.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the access-control entry.\"\n        },\n        \"selfLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The link to this access-control entry.\"\n        },\n        \"bucket\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the bucket.\"\n        },\n        \"object\": {\n\
  \          \"type\": [\"string\", \"null\"],\n          \"description\": \"The name of the object, if applied to an object.\"\n        },\n        \"generation\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The content generation of the object, if applied to an object.\"\n        },\n        \"entity\": {\n          \"type\": \"string\",\n          \"description\": \"The entity holding the permission.\",\n          \"examples\": [\"user-example@gmail.com\", \"allUsers\"]\n        },\n        \"role\": {\n          \"type\": \"string\",\n          \"description\": \"The access permission for the entity.\",\n          \"enum\": [\"OWNER\", \"READER\"]\n        },\n        \"email\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"email\",\n          \"description\": \"The email address associated with the entity, if any.\"\n        },\n        \"domain\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"\
  The domain associated with the entity, if any.\"\n        },\n        \"entityId\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The ID for the entity, if any.\"\n        },\n        \"etag\": {\n          \"type\": \"string\",\n          \"description\": \"HTTP 1.1 Entity tag for the access-control entry.\"\n        },\n        \"projectTeam\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"The project team associated with the entity, if any.\",\n          \"properties\": {\n            \"projectNumber\": {\n              \"type\": \"string\",\n              \"description\": \"The project number.\"\n            },\n            \"team\": {\n              \"type\": \"string\",\n              \"description\": \"The team.\",\n              \"enum\": [\"editors\", \"owners\", \"viewers\"]\n            }\n          }\n        }\n      }\n    },\n    \"IamConfiguration\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\"\
  : \"The bucket's IAM configuration, including uniform bucket-level access and public access prevention settings.\",\n      \"properties\": {\n        \"uniformBucketLevelAccess\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"The bucket's uniform bucket-level access configuration. When enabled, access is controlled exclusively through IAM policies and ACLs are disabled.\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether uniform bucket-level access is enabled. Once the lock time passes, this becomes permanent.\"\n            },\n            \"lockedTime\": {\n              \"type\": [\"string\", \"null\"],\n              \"format\": \"date-time\",\n              \"description\": \"The deadline for changing iamConfiguration.uniformBucketLevelAccess.enabled from true to false. After the deadline passes, the configuration becomes immutable.\"\n            }\n          }\n\
  \        },\n        \"publicAccessPrevention\": {\n          \"type\": \"string\",\n          \"description\": \"The bucket's public access prevention configuration. When set to enforced, prevents ACLs and IAM policies from granting public access.\",\n          \"enum\": [\"inherited\", \"enforced\"]\n        }\n      }\n    },\n    \"LifecycleRule\": {\n      \"type\": \"object\",\n      \"description\": \"A lifecycle management rule, which is made of an action to take and the condition(s) under which the action will be taken.\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"object\",\n          \"description\": \"The action to take when lifecycle conditions are met.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"Type of the action. Delete permanently deletes the object, SetStorageClass changes the storage class, and AbortIncompleteMultipartUpload aborts incomplete multipart uploads.\"\
  ,\n              \"enum\": [\"Delete\", \"SetStorageClass\", \"AbortIncompleteMultipartUpload\"]\n            },\n            \"storageClass\": {\n              \"type\": \"string\",\n              \"description\": \"Target storage class. Required only when the action type is SetStorageClass.\",\n              \"enum\": [\"STANDARD\", \"NEARLINE\", \"COLDLINE\", \"ARCHIVE\"]\n            }\n          },\n          \"required\": [\"type\"]\n        },\n        \"condition\": {\n          \"type\": \"object\",\n          \"description\": \"The condition(s) under which the action will be taken. All conditions must be met for the action to occur.\",\n          \"properties\": {\n            \"age\": {\n              \"type\": \"integer\",\n              \"description\": \"Age of an object in days. The condition is satisfied when an object reaches the specified age.\",\n              \"minimum\": 0,\n              \"examples\": [30, 90, 365]\n            },\n            \"createdBefore\": {\n\
  \              \"type\": \"string\",\n              \"format\": \"date\",\n              \"description\": \"A date in RFC 3339 format (YYYY-MM-DD). Objects created before midnight of this date satisfy the condition.\"\n            },\n            \"customTimeBefore\": {\n              \"type\": \"string\",\n              \"format\": \"date\",\n              \"description\": \"A date in RFC 3339 format (YYYY-MM-DD). Objects whose custom time is earlier than this date satisfy the condition.\"\n            },\n            \"daysSinceCustomTime\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of days elapsed since the user-specified custom time.\",\n              \"minimum\": 0\n            },\n            \"daysSinceNoncurrentTime\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of days elapsed since the noncurrent timestamp of an object. Relevant only for versioned objects.\",\n              \"minimum\": 0\n          \
  \  },\n            \"isLive\": {\n              \"type\": [\"boolean\", \"null\"],\n              \"description\": \"Relevant only for versioned objects. If true, this condition matches live objects; if false, it matches noncurrent objects.\"\n            },\n            \"matchesPattern\": {\n              \"type\": \"string\",\n              \"description\": \"A regular expression that satisfies the RE2 syntax. This condition is satisfied when the name of the object matches the pattern.\"\n            },\n            \"matchesPrefix\": {\n              \"type\": \"array\",\n              \"description\": \"Objects having any of the specified name prefixes satisfy this condition.\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"matchesSuffix\": {\n              \"type\": \"array\",\n              \"description\": \"Objects having any of the specified name suffixes satisfy this condition.\",\n              \"items\": {\n\
  \                \"type\": \"string\"\n              }\n            },\n            \"matchesStorageClass\": {\n              \"type\": \"array\",\n              \"description\": \"Objects having any of the storage classes specified by this condition satisfy this condition.\",\n              \"items\": {\n                \"type\": \"string\",\n                \"enum\": [\"STANDARD\", \"NEARLINE\", \"COLDLINE\", \"ARCHIVE\", \"MULTI_REGIONAL\", \"REGIONAL\", \"DURABLE_REDUCED_AVAILABILITY\"]\n              }\n            },\n            \"noncurrentTimeBefore\": {\n              \"type\": \"string\",\n              \"format\": \"date\",\n              \"description\": \"A date in RFC 3339 format (YYYY-MM-DD). Objects whose noncurrent time is earlier than this date satisfy the condition.\"\n            },\n            \"numNewerVersions\": {\n              \"type\": \"integer\",\n              \"description\": \"Relevant only for versioned objects. If the value is N, this condition is satisfied\
  \ when there are at least N versions (including the live version) newer than this version of the object.\",\n              \"minimum\": 0\n            }\n          }\n        }\n      }\n    },\n    \"CorsConfiguration\": {\n      \"type\": \"object\",\n      \"description\": \"A CORS configuration entry for the bucket.\",\n      \"properties\": {\n        \"origin\": {\n          \"type\": \"array\",\n          \"description\": \"The list of Origins eligible to receive CORS response headers. The value * is permitted as a wildcard.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"examples\": [[\"https://example.com\", \"https://app.example.com\"]]\n        },\n        \"method\": {\n          \"type\": \"array\",\n          \"description\": \"The list of HTTP methods on which to include CORS response headers (GET, OPTIONS, POST, etc.). The value * is permitted as a wildcard.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n\
  \          \"examples\": [[\"GET\", \"POST\", \"PUT\", \"DELETE\"]]\n        },\n        \"responseHeader\": {\n          \"type\": \"array\",\n          \"description\": \"The list of HTTP headers other than the simple response headers to give permission for the user-agent to share across domains.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"examples\": [[\"Content-Type\", \"x-goog-meta-*\"]]\n        },\n        \"maxAgeSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"The value, in seconds, to return in the Access-Control-Max-Age header used in preflight responses.\",\n          \"minimum\": 0,\n          \"examples\": [3600]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gcp-cloud-storage/refs/heads/main/json-schema/gcp-cloud-storage-bucket-schema.json
tags:
- Archival
- Backup
- Blob Storage
- Cloud Storage
- Data
- File Storage
- Google Cloud
- Object Storage
- Storage
title: Google Cloud Storage Bucket
---
