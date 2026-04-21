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
