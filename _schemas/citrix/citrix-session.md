---
description: Represents an active user session on a Citrix virtual desktop or application, including connection state and hosting machine information.
layout: schema
name: Citrix Session
properties_list:
- description: Unique identifier for the session
  name: id
  type: string
- description: Username of the session owner
  name: userName
  type: string
- description: Current session state
  name: state
  type: string
- description: When the session was established
  name: startTime
  type: string
- description: Name of the machine hosting the session
  name: machineName
  type: string
- description: Name of the client device connected to the session
  name: clientName
  type: string
- description: Applications currently running in the session
  name: applicationNames
  type: array
provider_name: Citrix
provider_slug: citrix
schema_file: json-schema/citrix-session-schema.json
slug: citrix-session
tags:
- Application Delivery
- Desktop-As-A-Service
- Networking
- Virtualization
- Workspace
title: Citrix Session
---
