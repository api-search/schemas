---
description: Schema for Windows 10 storage items including files (StorageFile) and folders (StorageFolder) as defined by the Windows.Storage namespace. Covers file properties, folder hierarchies, application data, and library management.
layout: schema
name: Windows 10 Storage Item
properties_list:
- description: Whether this is a file or folder (StorageItemTypes)
  name: itemType
  type: string
- description: Item name including extension for files
  name: name
  type: string
- description: User-friendly display name without extension
  name: displayName
  type: string
- description: Full file system path
  name: path
  type: string
- description: Date and time the item was created
  name: dateCreated
  type: string
- description: Date and time the item was last modified
  name: dateModified
  type: string
- description: File attributes (FileAttributes flags)
  name: attributes
  type: array
- description: ''
  name: fileProperties
  type: object
- description: ''
  name: folderProperties
  type: object
- description: ''
  name: provider
  type: object
- description: ''
  name: thumbnail
  type: object
provider_name: Microsoft Windows 10
provider_slug: microsoft-windows-10
schema_file: json-schema/microsoft-windows-10-storage-item-schema.json
slug: microsoft-windows-10-storage-item
source_filename: microsoft-windows-10-storage-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.microsoft.com/schemas/windows-10/storage-item.json\",\n  \"title\": \"Windows 10 Storage Item\",\n  \"description\": \"Schema for Windows 10 storage items including files (StorageFile) and folders (StorageFolder) as defined by the Windows.Storage namespace. Covers file properties, folder hierarchies, application data, and library management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"itemType\": {\n      \"type\": \"string\",\n      \"enum\": [\"File\", \"Folder\"],\n      \"description\": \"Whether this is a file or folder (StorageItemTypes)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Item name including extension for files\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"User-friendly display name without extension\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Full file system path\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the item was created\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the item was last modified\"\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"Normal\", \"ReadOnly\", \"Directory\", \"Archive\", \"Temporary\", \"LocallyIncomplete\"]\n      },\n      \"description\": \"File attributes (FileAttributes flags)\"\n    },\n    \"fileProperties\": {\n      \"$ref\": \"#/$defs/FileProperties\"\n    },\n    \"folderProperties\": {\n      \"$ref\": \"#/$defs/FolderProperties\"\n    },\n    \"provider\": {\n      \"$ref\": \"#/$defs/StorageProvider\"\n    },\n    \"thumbnail\": {\n      \"$ref\": \"#/$defs/Thumbnail\"\n    }\n  },\n  \"required\": [\"itemType\",\
  \ \"name\", \"path\"],\n  \"$defs\": {\n    \"FileProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties specific to files (StorageFile class)\",\n      \"properties\": {\n        \"fileType\": {\n          \"type\": \"string\",\n          \"description\": \"File extension (e.g., .jpg, .docx)\"\n        },\n        \"contentType\": {\n          \"type\": \"string\",\n          \"description\": \"MIME content type\"\n        },\n        \"size\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"minimum\": 0,\n          \"description\": \"File size in bytes\"\n        },\n        \"isAvailable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the file content is available locally (IStorageFilePropertiesWithAvailability)\"\n        },\n        \"basicProperties\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"dateModified\": {\n              \"type\": \"string\",\n    \
  \          \"format\": \"date-time\"\n            },\n            \"itemDate\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            },\n            \"size\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\"\n            }\n          }\n        },\n        \"imageProperties\": {\n          \"type\": \"object\",\n          \"description\": \"Image-specific properties (for image files)\",\n          \"properties\": {\n            \"width\": {\n              \"type\": \"integer\"\n            },\n            \"height\": {\n              \"type\": \"integer\"\n            },\n            \"cameraModel\": {\n              \"type\": \"string\"\n            },\n            \"cameraManufacturer\": {\n              \"type\": \"string\"\n            },\n            \"dateTaken\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            },\n            \"orientation\": {\n              \"type\"\
  : \"string\",\n              \"enum\": [\"Normal\", \"FlipHorizontal\", \"Rotate180\", \"FlipVertical\", \"Transpose\", \"Rotate270\", \"Transverse\", \"Rotate90\", \"Unspecified\"]\n            },\n            \"latitude\": {\n              \"type\": \"number\",\n              \"format\": \"double\"\n            },\n            \"longitude\": {\n              \"type\": \"number\",\n              \"format\": \"double\"\n            }\n          }\n        },\n        \"musicProperties\": {\n          \"type\": \"object\",\n          \"description\": \"Music-specific properties (for audio files)\",\n          \"properties\": {\n            \"artist\": {\n              \"type\": \"string\"\n            },\n            \"album\": {\n              \"type\": \"string\"\n            },\n            \"albumArtist\": {\n              \"type\": \"string\"\n            },\n            \"title\": {\n              \"type\": \"string\"\n            },\n            \"trackNumber\": {\n             \
  \ \"type\": \"integer\"\n            },\n            \"genre\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"duration\": {\n              \"type\": \"string\",\n              \"description\": \"Duration in ISO 8601 format\"\n            },\n            \"bitrate\": {\n              \"type\": \"integer\"\n            },\n            \"year\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"videoProperties\": {\n          \"type\": \"object\",\n          \"description\": \"Video-specific properties (for video files)\",\n          \"properties\": {\n            \"title\": {\n              \"type\": \"string\"\n            },\n            \"width\": {\n              \"type\": \"integer\"\n            },\n            \"height\": {\n              \"type\": \"integer\"\n            },\n            \"duration\": {\n              \"type\": \"string\"\
  \n            },\n            \"bitrate\": {\n              \"type\": \"integer\"\n            },\n            \"directors\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"year\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      }\n    },\n    \"FolderProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties specific to folders (StorageFolder class)\",\n      \"properties\": {\n        \"fileCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of files in the folder\"\n        },\n        \"folderCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of subfolders\"\n        },\n        \"totalSize\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Total size of all contents in bytes\"\n        }\n      }\n    },\n \
  \   \"StorageProvider\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the storage provider (StorageProvider class)\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Provider identifier\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Provider display name (e.g., This PC, OneDrive)\"\n        }\n      }\n    },\n    \"Thumbnail\": {\n      \"type\": \"object\",\n      \"description\": \"Thumbnail for the storage item\",\n      \"properties\": {\n        \"originalWidth\": {\n          \"type\": \"integer\"\n        },\n        \"originalHeight\": {\n          \"type\": \"integer\"\n        },\n        \"returnedSmallerCachedSize\": {\n          \"type\": \"boolean\"\n        },\n        \"contentType\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/json-schema/microsoft-windows-10-storage-item-schema.json
tags:
- Desktop
- Operating System
- UWP
- Win32
- Windows
title: Windows 10 Storage Item
---
