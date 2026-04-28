---
description: Represents a Webex device or room system, including its configuration, connection status, and workspace assignment.
layout: schema
name: Cisco Webex Device
properties_list:
- description: Unique identifier for the device.
  name: id
  type: string
- description: Display name of the device.
  name: displayName
  type: string
- description: Workspace ID the device is assigned to.
  name: workspaceId
  type: string
- description: Person ID the device is assigned to.
  name: personId
  type: string
- description: Organization ID the device belongs to.
  name: orgId
  type: string
- description: List of device capabilities.
  name: capabilities
  type: array
- description: List of device permissions.
  name: permissions
  type: array
- description: Current connection status of the device.
  name: connectionStatus
  type: string
- description: Product name of the device.
  name: product
  type: string
- description: Device type.
  name: type
  type: string
- description: Tags assigned to the device.
  name: tags
  type: array
- description: IP address of the device.
  name: ip
  type: string
- description: MAC address of the device.
  name: mac
  type: string
- description: Serial number of the device.
  name: serial
  type: string
- description: Software version running on the device.
  name: software
  type: string
- description: Upgrade channel for the device.
  name: upgradeChannel
  type: string
- description: Primary SIP URL of the device.
  name: primarySipUrl
  type: string
- description: SIP URLs assigned to the device.
  name: sipUrls
  type: array
- description: Error codes reported by the device.
  name: errorCodes
  type: array
- description: Date and time the device was created.
  name: created
  type: string
- description: Date and time the device was first seen.
  name: firstSeen
  type: string
- description: Date and time the device was last seen.
  name: lastSeen
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-device-schema.json
slug: cisco-webex-device
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Device
---
