---
description: FHIR R4 Patient resource as exposed by the Cigna Patient Access API. Aligned with the US Core Patient profile referenced by the HL7 Da Vinci PDex implementation guide.
layout: schema
name: CignaPatient
properties_list:
- description: ''
  name: resourceType
  type: string
- description: Logical identifier of the Patient resource.
  name: id
  type: string
- description: ''
  name: identifier
  type: array
- description: ''
  name: active
  type: boolean
- description: ''
  name: name
  type: array
- description: ''
  name: telecom
  type: array
- description: ''
  name: gender
  type: string
- description: ''
  name: birthDate
  type: string
- description: ''
  name: address
  type: array
- description: ''
  name: communication
  type: array
provider_name: Cigna
provider_slug: cigna
schema_file: json-schema/cigna-patient-schema.json
slug: cigna-patient
tags:
- CMS Interoperability
- Da Vinci
- Drug Formulary
- FHIR
- Health Insurance
- Healthcare
- Patient Access
- Provider Directory
- SMART on FHIR
title: CignaPatient
---
