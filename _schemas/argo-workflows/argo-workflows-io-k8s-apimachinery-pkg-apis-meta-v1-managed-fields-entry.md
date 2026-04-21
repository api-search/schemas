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
