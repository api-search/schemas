---
description: ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the resource that the fieldset applies to.
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.ManagedFieldsEntry
properties_list:
- description: 'APIVersion defines the version of this resource that this field set applies to. The format is "group/version" just like the top-level APIVersion field. It is necessary to track the version of a field '
  name: apiVersion
  type: string
- description: 'FieldsType is the discriminator for the different fields format and version. There is currently only one possible value: "FieldsV1"'
  name: fieldsType
  type: string
- description: FieldsV1 holds the first JSON version format as described in the "FieldsV1" type.
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
- description: Time is the timestamp of when the ManagedFields entry was added. The timestamp will also be updated if a field is added, the manager changes any of the owned fields value or removes a field. The times
  name: time
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-managed-fields-entry-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-managed-fields-entry
source_filename: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-managed-fields-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-managed-fields-entry-schema.json\",\n  \"title\": \"io.k8s.apimachinery.pkg.apis.meta.v1.ManagedFieldsEntry\",\n  \"description\": \"ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the resource that the fieldset applies to.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"description\": \"APIVersion defines the version of this resource that this field set applies to. The format is \\\"group/version\\\" just like the top-level APIVersion field. It is necessary to track the version of a field set because it cannot be automatically converted.\",\n      \"type\": \"string\"\n    },\n    \"fieldsType\": {\n      \"description\": \"FieldsType is the discriminator for the different fields format and version.\
  \ There is currently only one possible value: \\\"FieldsV1\\\"\",\n      \"type\": \"string\"\n    },\n    \"fieldsV1\": {\n      \"description\": \"FieldsV1 holds the first JSON version format as described in the \\\"FieldsV1\\\" type.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.FieldsV1\"\n    },\n    \"manager\": {\n      \"description\": \"Manager is an identifier of the workflow managing these fields.\",\n      \"type\": \"string\"\n    },\n    \"operation\": {\n      \"description\": \"Operation is the type of operation which lead to this ManagedFieldsEntry being created. The only valid values for this field are 'Apply' and 'Update'.\",\n      \"type\": \"string\"\n    },\n    \"subresource\": {\n      \"description\": \"Subresource is the name of the subresource used to update that object, or empty string if the object was updated through the main resource. The value of this field is used to distinguish between managers, even if they share the same name.\
  \ For example, a status update will be distinct from a regular update using the same manager name. Note that the APIVersion field is not related to the Subresource field and it always corresponds to the version of the main resource.\",\n      \"type\": \"string\"\n    },\n    \"time\": {\n      \"description\": \"Time is the timestamp of when the ManagedFields entry was added. The timestamp will also be updated if a field is added, the manager changes any of the owned fields value or removes a field. The timestamp does not update when a field is removed from the entry because another manager took it over.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-managed-fields-entry-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.ManagedFieldsEntry
---
