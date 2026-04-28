---
description: Represents a user in the Webex platform including profile information, contact details, roles, and licenses.
layout: schema
name: Cisco Webex Person
properties_list:
- description: Unique identifier for the person.
  name: id
  type: string
- description: Email addresses associated with the person.
  name: emails
  type: array
- description: Phone numbers for the person.
  name: phoneNumbers
  type: array
- description: SIP addresses of the person.
  name: sipAddresses
  type: array
- description: Webex Calling extension number.
  name: extension
  type: string
- description: Location ID for Webex Calling.
  name: locationId
  type: string
- description: Full display name of the person.
  name: displayName
  type: string
- description: Nickname of the person.
  name: nickName
  type: string
- description: First name of the person.
  name: firstName
  type: string
- description: Last name of the person.
  name: lastName
  type: string
- description: URL to the person's avatar image.
  name: avatar
  type: string
- description: Organization ID the person belongs to.
  name: orgId
  type: string
- description: Role IDs assigned to the person.
  name: roles
  type: array
- description: License IDs assigned to the person.
  name: licenses
  type: array
- description: Department of the person.
  name: department
  type: string
- description: Manager name of the person.
  name: manager
  type: string
- description: Person ID of the manager.
  name: managerId
  type: string
- description: Job title of the person.
  name: title
  type: string
- description: Physical addresses of the person.
  name: addresses
  type: array
- description: Date and time the person was created.
  name: created
  type: string
- description: Date and time the person was last modified.
  name: lastModified
  type: string
- description: Time zone of the person in IANA format.
  name: timezone
  type: string
- description: Date and time of the person's last activity.
  name: lastActivity
  type: string
- description: Webex site URLs associated with the person.
  name: siteUrls
  type: array
- description: Current presence status of the person.
  name: status
  type: string
- description: Type of the person account.
  name: type
  type: string
- description: Whether the invite is pending acceptance.
  name: invitePending
  type: boolean
- description: Whether the person's login is enabled.
  name: loginEnabled
  type: boolean
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-person-schema.json
slug: cisco-webex-person
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Person
---
