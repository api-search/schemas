---
description: Defines a maintenance track that determines which Amazon Redshift version to apply during a maintenance window. If the value for <code>MaintenanceTrack</code> is <code>current</code>, the cluster is updated to the most recently certified maintenance release. If the value is <code>trailing</code>, the cluster is updated to the previously certified maintenance release.
layout: schema
name: MaintenanceTrack
properties_list:
- description: ''
  name: MaintenanceTrackName
  type: object
- description: ''
  name: DatabaseVersion
  type: object
- description: ''
  name: UpdateTargets
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-maintenance-track-schema.json
slug: redshift-maintenance-track
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: MaintenanceTrack
---
