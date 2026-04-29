---
description: ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the resource that the fieldset applies to.
layout: schema
name: v1ManagedFieldsEntry
properties_list:
- description: 'APIVersion defines the version of this resource that this field set applies to. The format is "group/version" just like the top-level APIVersion field. It is necessary to track the version of a field '
  name: apiVersion
  type: string
- description: ''
  name: fieldsType
  type: string
- description: ''
  name: fieldsV1
  type: object
- description: Manager is an identifier of the workflow managing these fields.
  name: manager
  type: string
- description: Operation is the type of operation which lead to this ManagedFieldsEntry being created. The only valid values for this field are 'Apply' and 'Update'.
  name: operation
  type: string
- description: Subresource is the name of the subresource used to update that object, or empty string if the object was updated through the main resource. The value of this field is used to distinguish between manag
  name: subresource
  type: string
- description: ''
  name: time
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1-managed-fields-entry-schema.json
slug: argo-cd-v1-managed-fields-entry
source_filename: argo-cd-v1-managed-fields-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-managed-fields-entry-schema.json\",\n  \"title\": \"v1ManagedFieldsEntry\",\n  \"description\": \"ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the resource\\nthat the fieldset applies to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"APIVersion defines the version of this resource that this field set\\napplies to. The format is \\\"group/version\\\" just like the top-level\\nAPIVersion field. It is necessary to track the version of a field\\nset because it cannot be automatically converted.\",\n      \"type\": \"string\"\n    },\n    \"fieldsType\": {\n      \"type\": \"string\",\n      \"title\": \"FieldsType is the discriminator for the different fields format and version.\\nThere is currently only one possible value:\
  \ \\\"FieldsV1\\\"\"\n    },\n    \"fieldsV1\": {\n      \"$ref\": \"#/definitions/v1FieldsV1\"\n    },\n    \"manager\": {\n      \"description\": \"Manager is an identifier of the workflow managing these fields.\",\n      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"description\": \"Operation is the type of operation which lead to this ManagedFieldsEntry being created.\\nThe only valid values for this field are 'Apply' and 'Update'.\",\n      \"type\": \"string\"\n    },\n    \"subresource\": {\n      \"description\": \"Subresource is the name of the subresource used to update that object, or\\nempty string if the object was updated through the main resource. The\\nvalue of this field is used to distinguish between managers, even if they\\nshare the same name. For example, a status update will be distinct from a\\nregular update using the same manager name.\\nNote that the APIVersion field is not related to the Subresource field and\\nit always corresponds to the version\
  \ of the main resource.\",\n      \"type\": \"string\"\n    },\n    \"time\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1-managed-fields-entry-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1ManagedFieldsEntry
---
