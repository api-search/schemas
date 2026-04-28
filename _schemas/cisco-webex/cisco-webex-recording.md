---
description: Represents a Webex meeting recording including metadata, download links, and playback information.
layout: schema
name: Cisco Webex Recording
properties_list:
- description: Unique identifier for the recording.
  name: id
  type: string
- description: The meeting ID associated with the recording.
  name: meetingId
  type: string
- description: The topic or title of the recording.
  name: topic
  type: string
- description: Date and time the recording was created.
  name: createTime
  type: string
- description: Date and time the recording was made.
  name: timeRecorded
  type: string
- description: URL to download the recording.
  name: downloadUrl
  type: string
- description: URL to play back the recording.
  name: playbackUrl
  type: string
- description: Password required to access the recording.
  name: password
  type: string
- description: Format of the recording file.
  name: format
  type: string
- description: Webex service type the recording originated from.
  name: serviceType
  type: string
- description: Duration of the recording in seconds.
  name: durationSeconds
  type: integer
- description: Size of the recording file in bytes.
  name: sizeBytes
  type: integer
- description: Current status of the recording.
  name: status
  type: string
- description: Temporary download links with expiration timestamps.
  name: temporaryDirectDownloadLinks
  type: object
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-recording-schema.json
slug: cisco-webex-recording
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Recording
---
