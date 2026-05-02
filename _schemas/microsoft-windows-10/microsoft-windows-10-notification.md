---
description: Schema for Windows 10 toast, tile, and badge notifications as defined by the Windows.UI.Notifications namespace. Covers ToastNotification, TileNotification, BadgeNotification, and ScheduledToastNotification data models.
layout: schema
name: Windows 10 Notification
properties_list:
- description: The type of notification
  name: notificationType
  type: string
- description: Tag identifier for the notification, used for updating and removing specific notifications
  name: tag
  type: string
- description: Group identifier for organizing related notifications
  name: group
  type: string
- description: The time when the notification expires and is removed from the action center
  name: expirationTime
  type: string
- description: Whether to suppress the popup toast and send directly to the action center
  name: suppressPopup
  type: boolean
- description: Notification priority level (ToastNotificationPriority)
  name: priority
  type: string
- description: Whether the notification can be mirrored to other devices
  name: notificationMirroring
  type: string
- description: ''
  name: visual
  type: object
- description: ''
  name: actions
  type: object
- description: ''
  name: audio
  type: object
- description: NotificationData for data binding with key-value pairs
  name: data
  type: object
- description: ''
  name: schedule
  type: object
provider_name: Microsoft Windows 10
provider_slug: microsoft-windows-10
schema_file: json-schema/microsoft-windows-10-notification-schema.json
slug: microsoft-windows-10-notification
source_filename: microsoft-windows-10-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.microsoft.com/schemas/windows-10/notification.json\",\n  \"title\": \"Windows 10 Notification\",\n  \"description\": \"Schema for Windows 10 toast, tile, and badge notifications as defined by the Windows.UI.Notifications namespace. Covers ToastNotification, TileNotification, BadgeNotification, and ScheduledToastNotification data models.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"toast\", \"tile\", \"badge\", \"tileFlyout\"],\n      \"description\": \"The type of notification\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"maxLength\": 16,\n      \"description\": \"Tag identifier for the notification, used for updating and removing specific notifications\"\n    },\n    \"group\": {\n      \"type\": \"string\",\n      \"maxLength\": 16,\n      \"description\": \"Group identifier\
  \ for organizing related notifications\"\n    },\n    \"expirationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the notification expires and is removed from the action center\"\n    },\n    \"suppressPopup\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to suppress the popup toast and send directly to the action center\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\"Default\", \"High\"],\n      \"default\": \"Default\",\n      \"description\": \"Notification priority level (ToastNotificationPriority)\"\n    },\n    \"notificationMirroring\": {\n      \"type\": \"string\",\n      \"enum\": [\"Allowed\", \"Disabled\"],\n      \"default\": \"Allowed\",\n      \"description\": \"Whether the notification can be mirrored to other devices\"\n    },\n    \"visual\": {\n      \"$ref\": \"#/$defs/NotificationVisual\"\n    },\n    \"actions\": {\n    \
  \  \"$ref\": \"#/$defs/NotificationActions\"\n    },\n    \"audio\": {\n      \"$ref\": \"#/$defs/NotificationAudio\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"NotificationData for data binding with key-value pairs\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/$defs/NotificationSchedule\"\n    }\n  },\n  \"required\": [\"notificationType\", \"visual\"],\n  \"$defs\": {\n    \"NotificationVisual\": {\n      \"type\": \"object\",\n      \"description\": \"Visual content of the notification (NotificationVisual class)\",\n      \"properties\": {\n        \"bindings\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/NotificationBinding\"\n          },\n          \"description\": \"One or more binding elements defining the notification content\"\n        }\n      },\n      \"required\": [\"bindings\"]\n    },\n    \"NotificationBinding\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"A binding element defining notification content for a specific template\",\n      \"properties\": {\n        \"template\": {\n          \"type\": \"string\",\n          \"description\": \"Template type (ToastGeneric, TileSmall, TileMedium, TileWide, TileLarge)\",\n          \"examples\": [\"ToastGeneric\", \"TileMedium\", \"TileWide\"]\n        },\n        \"texts\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/AdaptiveText\"\n          },\n          \"description\": \"Text elements in the binding\"\n        },\n        \"images\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/AdaptiveImage\"\n          },\n          \"description\": \"Image elements in the binding\"\n        },\n        \"attributionText\": {\n          \"type\": \"string\",\n          \"description\": \"Attribution text displayed at the bottom of the notification\"\n  \
  \      },\n        \"displayTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Custom timestamp to display instead of the notification delivery time\"\n        }\n      },\n      \"required\": [\"template\"]\n    },\n    \"AdaptiveText\": {\n      \"type\": \"object\",\n      \"description\": \"Text content element (AdaptiveNotificationText class)\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The text content\"\n        },\n        \"hintStyle\": {\n          \"type\": \"string\",\n          \"enum\": [\"caption\", \"captionSubtle\", \"body\", \"bodySubtle\", \"base\", \"baseSubtle\", \"subtitle\", \"subtitleSubtle\", \"title\", \"titleSubtle\", \"titleNumeral\", \"subheader\", \"subheaderSubtle\", \"subheaderNumeral\", \"header\", \"headerSubtle\", \"headerNumeral\"],\n          \"description\": \"Text style hint\"\n        },\n        \"hintMaxLines\"\
  : {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Maximum number of lines for this text element\"\n        },\n        \"hintWrap\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether text wrapping is enabled\"\n        },\n        \"hintAlign\": {\n          \"type\": \"string\",\n          \"enum\": [\"auto\", \"left\", \"center\", \"right\"],\n          \"description\": \"Text alignment\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"BCP-47 language tag\"\n        }\n      },\n      \"required\": [\"content\"]\n    },\n    \"AdaptiveImage\": {\n      \"type\": \"object\",\n      \"description\": \"Image content element for notifications\",\n      \"properties\": {\n        \"src\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Image source URI (ms-appx:///,  ms-appdata:///local/, or http/https)\"\n        },\n  \
  \      \"placement\": {\n          \"type\": \"string\",\n          \"enum\": [\"inline\", \"appLogoOverride\", \"hero\"],\n          \"default\": \"inline\",\n          \"description\": \"Image placement in the notification\"\n        },\n        \"hintCrop\": {\n          \"type\": \"string\",\n          \"enum\": [\"none\", \"circle\"],\n          \"default\": \"none\",\n          \"description\": \"Cropping applied to the image\"\n        },\n        \"alt\": {\n          \"type\": \"string\",\n          \"description\": \"Alternative text for accessibility\"\n        },\n        \"addImageQuery\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to append image query parameters for scale/contrast\"\n        }\n      },\n      \"required\": [\"src\"]\n    },\n    \"NotificationActions\": {\n      \"type\": \"object\",\n      \"description\": \"Interactive actions in a toast notification\",\n      \"properties\": {\n        \"inputs\": {\n          \"type\"\
  : \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/NotificationInput\"\n          },\n          \"maxItems\": 5,\n          \"description\": \"Input fields (up to 5)\"\n        },\n        \"buttons\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/NotificationButton\"\n          },\n          \"maxItems\": 5,\n          \"description\": \"Action buttons (up to 5)\"\n        }\n      }\n    },\n    \"NotificationInput\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Input identifier used to retrieve the value\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"selection\"],\n          \"description\": \"Input type\"\n        },\n        \"placeHolderContent\": {\n          \"type\": \"string\",\n          \"description\": \"Placeholder text for text inputs\"\n        },\n        \"title\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Label displayed above the input\"\n        },\n        \"defaultInput\": {\n          \"type\": \"string\",\n          \"description\": \"Default value\"\n        },\n        \"selections\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\"\n              },\n              \"content\": {\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\"id\", \"content\"]\n          },\n          \"description\": \"Selection options (for type=selection)\"\n        }\n      },\n      \"required\": [\"id\", \"type\"]\n    },\n    \"NotificationButton\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"Button label text\"\n        },\n        \"arguments\": {\n \
  \         \"type\": \"string\",\n          \"description\": \"Arguments passed to the app when the button is clicked\"\n        },\n        \"activationType\": {\n          \"type\": \"string\",\n          \"enum\": [\"foreground\", \"background\", \"protocol\", \"system\"],\n          \"default\": \"foreground\",\n          \"description\": \"How the app is activated when the button is clicked\"\n        },\n        \"imageUri\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Icon image for the button\"\n        },\n        \"inputId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the input field next to this button\"\n        }\n      },\n      \"required\": [\"content\", \"arguments\"]\n    },\n    \"NotificationAudio\": {\n      \"type\": \"object\",\n      \"description\": \"Audio settings for a toast notification\",\n      \"properties\": {\n        \"src\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Audio file URI (ms-winsoundevent: or ms-appx:/// or ms-appdata:///)\",\n          \"examples\": [\"ms-winsoundevent:Notification.Default\", \"ms-winsoundevent:Notification.Mail\"]\n        },\n        \"loop\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether the audio should loop\"\n        },\n        \"silent\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether the notification should be silent\"\n        }\n      }\n    },\n    \"NotificationSchedule\": {\n      \"type\": \"object\",\n      \"description\": \"Scheduling information for scheduled toast notifications\",\n      \"properties\": {\n        \"deliveryTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The time to deliver the notification\"\n        },\n        \"snoozeInterval\": {\n          \"type\": \"integer\",\n          \"minimum\"\
  : 1,\n          \"description\": \"Snooze interval in minutes\"\n        },\n        \"maximumSnoozeCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 5,\n          \"description\": \"Maximum number of snoozes allowed\"\n        }\n      },\n      \"required\": [\"deliveryTime\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/json-schema/microsoft-windows-10-notification-schema.json
tags:
- Desktop
- Operating System
- UWP
- Win32
- Windows
title: Windows 10 Notification
---
