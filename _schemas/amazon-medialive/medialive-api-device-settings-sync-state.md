---
description: The status of the action to synchronize the device configuration. If you change the configuration of the input device (for example, the maximum bitrate), MediaLive sends the new data to the device. The device might not update itself immediately. SYNCED means the device has updated its configuration. SYNCING means that it has not updated its configuration.
layout: schema
name: DeviceSettingsSyncState
properties_list: []
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-device-settings-sync-state-schema.json
slug: medialive-api-device-settings-sync-state
source_filename: medialive-api-device-settings-sync-state-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-device-settings-sync-state-schema.json\",\n  \"title\": \"DeviceSettingsSyncState\",\n  \"description\": \"The status of the action to synchronize the device configuration. If you change the configuration of the input device (for example, the maximum bitrate), MediaLive sends the new data to the device. The device might not update itself immediately. SYNCED means the device has updated its configuration. SYNCING means that it has not updated its configuration.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SYNCED\",\n    \"SYNCING\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-device-settings-sync-state-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DeviceSettingsSyncState
---
