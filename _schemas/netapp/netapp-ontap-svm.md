---
description: A storage virtual machine (SVM), also known as a vserver, is a secure virtual storage server that provides isolated data access to clients. Each SVM has its own set of volumes, network interfaces, and protocol configurations.
layout: schema
name: Svm
properties_list:
- description: SVM UUID
  name: uuid
  type: string
- description: SVM name (unique within the cluster)
  name: name
  type: string
- description: SVM operational state
  name: state
  type: string
- description: SVM subtype
  name: subtype
  type: string
- description: Default language encoding for volumes in the SVM
  name: language
  type: string
- description: Optional comment or description for the SVM
  name: comment
  type: string
- description: IPspace associated with the SVM
  name: ipspace
  type: object
- description: Aggregates assigned to the SVM for volume provisioning
  name: aggregates
  type: array
- description: Network interfaces configured for the SVM
  name: ip_interfaces
  type: array
- description: NFS protocol configuration
  name: nfs
  type: object
- description: CIFS/SMB protocol configuration
  name: cifs
  type: object
- description: iSCSI protocol configuration
  name: iscsi
  type: object
- description: Fibre Channel Protocol configuration
  name: fcp
  type: object
- description: NVMe over Fabrics protocol configuration
  name: nvme
  type: object
- description: Default snapshot policy for the SVM
  name: snapshot_policy
  type: object
- description: DNS configuration for the SVM
  name: dns
  type: object
- description: SSL/TLS certificate for the SVM
  name: certificate
  type: object
- description: Maximum number of volumes allowed on the SVM
  name: max_volumes
  type: string
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-svm-schema.json
slug: netapp-ontap-svm
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Svm\",\n  \"type\": \"object\",\n  \"description\": \"A storage virtual machine (SVM), also known as a vserver, is a secure virtual storage server that provides isolated data access to clients. Each SVM has its own set of volumes, network interfaces, and protocol configurations.\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"SVM UUID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"SVM name (unique within the cluster)\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"SVM operational state\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"SVM subtype\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Default language encoding for volumes in the SVM\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n  \
  \    \"description\": \"Optional comment or description for the SVM\"\n    },\n    \"ipspace\": {\n      \"type\": \"object\",\n      \"description\": \"IPspace associated with the SVM\"\n    },\n    \"aggregates\": {\n      \"type\": \"array\",\n      \"description\": \"Aggregates assigned to the SVM for volume provisioning\"\n    },\n    \"ip_interfaces\": {\n      \"type\": \"array\",\n      \"description\": \"Network interfaces configured for the SVM\"\n    },\n    \"nfs\": {\n      \"type\": \"object\",\n      \"description\": \"NFS protocol configuration\"\n    },\n    \"cifs\": {\n      \"type\": \"object\",\n      \"description\": \"CIFS/SMB protocol configuration\"\n    },\n    \"iscsi\": {\n      \"type\": \"object\",\n      \"description\": \"iSCSI protocol configuration\"\n    },\n    \"fcp\": {\n      \"type\": \"object\",\n      \"description\": \"Fibre Channel Protocol configuration\"\n    },\n    \"nvme\": {\n      \"type\": \"object\",\n      \"description\": \"NVMe over\
  \ Fabrics protocol configuration\"\n    },\n    \"snapshot_policy\": {\n      \"type\": \"object\",\n      \"description\": \"Default snapshot policy for the SVM\"\n    },\n    \"dns\": {\n      \"type\": \"object\",\n      \"description\": \"DNS configuration for the SVM\"\n    },\n    \"certificate\": {\n      \"type\": \"object\",\n      \"description\": \"SSL/TLS certificate for the SVM\"\n    },\n    \"max_volumes\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum number of volumes allowed on the SVM\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-svm-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: Svm
---
