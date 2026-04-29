---
description: The properties of a container.
layout: schema
name: ContainerProperties
properties_list:
- description: The hasImmutabilityPolicy public property is set to true by SRP if ImmutabilityPolicy has been created for this container. The hasImmutabilityPolicy public property is set to false by SRP if Immutabil
  name: hasImmutabilityPolicy
  type: boolean
- description: 'The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. '
  name: hasLegalHold
  type: boolean
- description: The ImmutabilityPolicy property of the container.
  name: immutabilityPolicy
  type: object
- description: Returns the date and time the container was last modified.
  name: lastModifiedTime
  type: string
- description: Specifies whether the lease on a container is of infinite or fixed duration, only when the container is leased.
  name: leaseDuration
  type: string
- description: Lease state of the container.
  name: leaseState
  type: string
- description: The lease status of the container.
  name: leaseStatus
  type: string
- description: The LegalHold property of the container.
  name: legalHold
  type: object
- description: A name-value pair to associate with the container as metadata.
  name: metadata
  type: object
- description: Specifies whether data in the container may be accessed publicly and the level of access.
  name: publicAccess
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-container-properties-schema.json
slug: azure-storage-accounts-container-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-container-properties-schema.json\",\n  \"title\": \"ContainerProperties\",\n  \"description\": \"The properties of a container.\",\n  \"properties\": {\n    \"hasImmutabilityPolicy\": {\n      \"description\": \"The hasImmutabilityPolicy public property is set to true by SRP if ImmutabilityPolicy has been created for this container. The hasImmutabilityPolicy public property is set to false by SRP if ImmutabilityPolicy has not been created for this container.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"hasLegalHold\": {\n      \"description\": \"The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. There\
  \ can be a maximum of 1000 blob containers with hasLegalHold=true for a given account.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"immutabilityPolicy\": {\n      \"$ref\": \"#/definitions/ImmutabilityPolicyProperties\",\n      \"description\": \"The ImmutabilityPolicy property of the container.\",\n      \"readOnly\": true,\n      \"x-ms-client-name\": \"ImmutabilityPolicy\"\n    },\n    \"lastModifiedTime\": {\n      \"description\": \"Returns the date and time the container was last modified.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"leaseDuration\": {\n      \"description\": \"Specifies whether the lease on a container is of infinite or fixed duration, only when the container is leased.\",\n      \"enum\": [\n        \"Infinite\",\n        \"Fixed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\"\
  : \"LeaseDuration\"\n      }\n    },\n    \"leaseState\": {\n      \"description\": \"Lease state of the container.\",\n      \"enum\": [\n        \"Available\",\n        \"Leased\",\n        \"Expired\",\n        \"Breaking\",\n        \"Broken\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"LeaseState\"\n      }\n    },\n    \"leaseStatus\": {\n      \"description\": \"The lease status of the container.\",\n      \"enum\": [\n        \"Locked\",\n        \"Unlocked\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"LeaseStatus\"\n      }\n    },\n    \"legalHold\": {\n      \"$ref\": \"#/definitions/LegalHoldProperties\",\n      \"description\": \"The LegalHold property of the container.\",\n      \"readOnly\": true\n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\"\
  : \"string\"\n      },\n      \"description\": \"A name-value pair to associate with the container as metadata.\",\n      \"type\": \"object\"\n    },\n    \"publicAccess\": {\n      \"description\": \"Specifies whether data in the container may be accessed publicly and the level of access.\",\n      \"enum\": [\n        \"Container\",\n        \"Blob\",\n        \"None\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"PublicAccess\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-container-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ContainerProperties
---
