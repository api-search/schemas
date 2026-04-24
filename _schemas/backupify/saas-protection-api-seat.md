---
description: A licensed or unlicensed seat (user, mailbox, site, or team)
layout: schema
name: Seat
properties_list:
- description: Remote identifier for the seat in the source system
  name: remoteId
  type: string
- description: Display name of the seat
  name: displayName
  type: string
- description: Email address for user seats
  name: email
  type: string
- description: Type of seat
  name: seatType
  type: string
- description: Current license status
  name: licenseStatus
  type: string
- description: Timestamp of last successful backup
  name: lastBackup
  type: string
provider_name: Backupify
provider_slug: backupify
schema_file: json-schema/saas-protection-api-seat-schema.json
slug: saas-protection-api-seat
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
title: Seat
---
