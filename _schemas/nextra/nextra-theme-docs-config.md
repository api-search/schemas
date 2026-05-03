---
description: Configuration props for the nextra-theme-docs Layout component. Passed as React props to the <Layout> component in the root layout.tsx of a Nextra docs site. Controls sidebar behavior, navigation bar, table of contents, dark mode, edit links, feedback, i18n language switching, theming, and footer.
layout: schema
name: Nextra Docs Theme Layout Configuration
properties_list:
- description: Page map list. The result of the getPageMap(route = '/') call from the nextra/page-map module. Required by the Layout component to build the sidebar and navigation.
  name: pageMap
  type: array
- description: Rendered Banner component. Displayed at the top of every page. E.g. <Banner {...bannerProps} />.
  name: banner
  type: object
- description: Page content rendered inside the layout. Passed automatically by Next.js.
  name: children
  type: object
- description: Hide or show the copy page content button that copies the entire page markdown content to the clipboard.
  name: copyPageButton
  type: boolean
- description: Show or hide the dark mode select button in the navbar.
  name: darkMode
  type: boolean
- description: Base URL of the documentation repository on GitHub. Used to generate the edit this page and feedback links.
  name: docsRepositoryBase
  type: string
- description: Content of the edit link shown at the bottom of each page. Defaults to the string 'Edit this page'.
  name: editLink
  type: object
- description: ''
  name: feedback
  type: object
- description: Rendered Footer component. E.g. <Footer {...footerProps} />.
  name: footer
  type: object
- description: Options to configure the language dropdown for internationalized docs sites.
  name: i18n
  type: array
- description: Component to render the last updated timestamp. Must be a <LastUpdated /> component from nextra-theme-docs.
  name: lastUpdated
  type: object
- description: Rendered Navbar component. E.g. <Navbar {...navbarProps} />.
  name: navbar
  type: object
- description: Enable or disable previous/next page navigation links at the bottom of the page.
  name: navigation
  type: object
- description: ''
  name: nextThemes
  type: object
- description: Rendered Search component. E.g. <Search {...searchProps} />. Defaults to the built-in Pagefind-powered search.
  name: search
  type: object
- description: ''
  name: sidebar
  type: object
- description: ''
  name: themeSwitch
  type: object
- description: ''
  name: toc
  type: object
provider_name: Nextra
provider_slug: nextra
schema_file: json-schema/nextra-theme-docs-config-schema.json
slug: nextra-theme-docs-config
source_filename: nextra-theme-docs-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://nextra.site/schemas/nextra/nextra-theme-docs-config.json\",\n  \"title\": \"Nextra Docs Theme Layout Configuration\",\n  \"description\": \"Configuration props for the nextra-theme-docs Layout component. Passed as React props to the <Layout> component in the root layout.tsx of a Nextra docs site. Controls sidebar behavior, navigation bar, table of contents, dark mode, edit links, feedback, i18n language switching, theming, and footer.\",\n  \"type\": \"object\",\n  \"required\": [\"pageMap\"],\n  \"properties\": {\n    \"pageMap\": {\n      \"type\": \"array\",\n      \"description\": \"Page map list. The result of the getPageMap(route = '/') call from the nextra/page-map module. Required by the Layout component to build the sidebar and navigation.\",\n      \"items\": {\n        \"description\": \"A PageMapItem representing a file, folder, or meta entry in the Nextra page tree.\"\n  \
  \    }\n    },\n    \"banner\": {\n      \"description\": \"Rendered Banner component. Displayed at the top of every page. E.g. <Banner {...bannerProps} />.\"\n    },\n    \"children\": {\n      \"description\": \"Page content rendered inside the layout. Passed automatically by Next.js.\"\n    },\n    \"copyPageButton\": {\n      \"type\": \"boolean\",\n      \"description\": \"Hide or show the copy page content button that copies the entire page markdown content to the clipboard.\",\n      \"default\": true\n    },\n    \"darkMode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Show or hide the dark mode select button in the navbar.\",\n      \"default\": true\n    },\n    \"docsRepositoryBase\": {\n      \"type\": \"string\",\n      \"pattern\": \"^https://\",\n      \"description\": \"Base URL of the documentation repository on GitHub. Used to generate the edit this page and feedback links.\",\n      \"default\": \"https://github.com/shuding/nextra\"\n    },\n    \"editLink\"\
  : {\n      \"description\": \"Content of the edit link shown at the bottom of each page. Defaults to the string 'Edit this page'.\",\n      \"default\": \"Edit this page\"\n    },\n    \"feedback\": {\n      \"$ref\": \"#/$defs/FeedbackConfig\"\n    },\n    \"footer\": {\n      \"description\": \"Rendered Footer component. E.g. <Footer {...footerProps} />.\"\n    },\n    \"i18n\": {\n      \"type\": \"array\",\n      \"description\": \"Options to configure the language dropdown for internationalized docs sites.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/I18nLocaleEntry\"\n      },\n      \"default\": []\n    },\n    \"lastUpdated\": {\n      \"description\": \"Component to render the last updated timestamp. Must be a <LastUpdated /> component from nextra-theme-docs.\",\n      \"default\": \"<LastUpdated />\"\n    },\n    \"navbar\": {\n      \"description\": \"Rendered Navbar component. E.g. <Navbar {...navbarProps} />.\"\n    },\n    \"navigation\": {\n      \"description\":\
  \ \"Enable or disable previous/next page navigation links at the bottom of the page.\",\n      \"oneOf\": [\n        {\n          \"type\": \"boolean\",\n          \"description\": \"Pass true to enable both prev and next links, false to disable both.\"\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"Fine-grained control over prev and next navigation links.\",\n          \"required\": [\"next\", \"prev\"],\n          \"properties\": {\n            \"next\": {\n              \"type\": \"boolean\",\n              \"description\": \"Show or hide the next page navigation link.\"\n            },\n            \"prev\": {\n              \"type\": \"boolean\",\n              \"description\": \"Show or hide the previous page navigation link.\"\n            }\n          },\n          \"additionalProperties\": false\n        }\n      ],\n      \"default\": true\n    },\n    \"nextThemes\": {\n      \"$ref\": \"#/$defs/NextThemesConfig\"\n    },\n    \"search\"\
  : {\n      \"description\": \"Rendered Search component. E.g. <Search {...searchProps} />. Defaults to the built-in Pagefind-powered search.\",\n      \"default\": \"<Search />\"\n    },\n    \"sidebar\": {\n      \"$ref\": \"#/$defs/SidebarConfig\"\n    },\n    \"themeSwitch\": {\n      \"$ref\": \"#/$defs/ThemeSwitchConfig\"\n    },\n    \"toc\": {\n      \"$ref\": \"#/$defs/TocConfig\"\n    }\n  },\n  \"$defs\": {\n    \"FeedbackConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for the feedback link shown at the bottom of documentation pages.\",\n      \"properties\": {\n        \"content\": {\n          \"description\": \"Content of the feedback link rendered to the user.\",\n          \"default\": \"Question? Give us feedback\"\n        },\n        \"labels\": {\n          \"type\": \"string\",\n          \"description\": \"Comma-separated GitHub issue labels applied when a new feedback issue is created.\",\n          \"default\": \"feedback\"\n    \
  \    },\n        \"link\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Custom URL for the feedback link. Defaults to the GitHub issue creation form for the docs repository with the page title prefilled.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"I18nLocaleEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A single locale entry for the i18n language dropdown.\",\n      \"required\": [\"locale\", \"name\"],\n      \"properties\": {\n        \"locale\": {\n          \"type\": \"string\",\n          \"description\": \"The locale code as defined in the i18n.locales field in next.config. E.g. 'en', 'zh-CN'.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable locale name displayed in the dropdown. E.g. 'English', '中文'.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"NextThemesConfig\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Configuration passed to the next-themes ThemeProvider. Controls how the theme class is applied and default theme behavior.\",\n      \"properties\": {\n        \"attribute\": {\n          \"description\": \"HTML attribute to apply the theme to. Can be 'class' or a data-* attribute, or an array of attributes.\",\n          \"oneOf\": [\n            {\n              \"type\": \"string\",\n              \"pattern\": \"^(class|data-.+)$\",\n              \"description\": \"Single attribute: 'class' or a data-* attribute.\"\n            },\n            {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\",\n                \"pattern\": \"^(class|data-.+)$\"\n              },\n              \"description\": \"Array of attributes.\"\n            }\n          ],\n          \"default\": \"class\"\n        },\n        \"defaultTheme\": {\n          \"type\": \"string\",\n          \"description\": \"Default\
  \ theme name on first load.\",\n          \"default\": \"system\"\n        },\n        \"disableTransitionOnChange\": {\n          \"type\": \"boolean\",\n          \"description\": \"Disable CSS transitions when switching themes to prevent a flash of unstyled content.\",\n          \"default\": true\n        },\n        \"forcedTheme\": {\n          \"type\": \"string\",\n          \"description\": \"Force a specific theme for all pages, overriding user preference.\"\n        },\n        \"storageKey\": {\n          \"type\": \"string\",\n          \"description\": \"Key used to persist the selected theme in localStorage.\",\n          \"default\": \"theme\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"SidebarConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for the sidebar navigation panel.\",\n      \"properties\": {\n        \"autoCollapse\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, automatically\
  \ collapse inactive folders above the defaultMenuCollapseLevel.\"\n        },\n        \"defaultMenuCollapseLevel\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Folder nesting level at which the sidebar menu is collapsed by default.\",\n          \"default\": 2\n        },\n        \"defaultOpen\": {\n          \"type\": \"boolean\",\n          \"description\": \"Show or hide the sidebar by default on page load.\",\n          \"default\": true\n        },\n        \"toggleButton\": {\n          \"type\": \"boolean\",\n          \"description\": \"Show or hide the sidebar toggle button.\",\n          \"default\": true\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"ThemeSwitchConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Translation strings for the theme switch dropdown options.\",\n      \"properties\": {\n        \"dark\": {\n          \"type\": \"string\",\n          \"description\": \"Label\
  \ for the dark mode option.\",\n          \"default\": \"Dark\"\n        },\n        \"light\": {\n          \"type\": \"string\",\n          \"description\": \"Label for the light mode option.\",\n          \"default\": \"Light\"\n        },\n        \"system\": {\n          \"type\": \"string\",\n          \"description\": \"Label for the system/auto theme option.\",\n          \"default\": \"System\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"TocConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for the table of contents sidebar panel.\",\n      \"properties\": {\n        \"backToTop\": {\n          \"description\": \"Text or element for the back-to-top button at the bottom of the TOC.\",\n          \"default\": \"Scroll to top\"\n        },\n        \"extraContent\": {\n          \"description\": \"Extra content rendered below the TOC entries.\"\n        },\n        \"float\": {\n          \"type\": \"boolean\",\n      \
  \    \"description\": \"Float the TOC panel next to the main content.\",\n          \"default\": true\n        },\n        \"title\": {\n          \"description\": \"Title rendered above the TOC entries.\",\n          \"default\": \"On This Page\"\n        }\n      },\n      \"additionalProperties\": false\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nextra/refs/heads/main/json-schema/nextra-theme-docs-config-schema.json
tags:
- Documentation
- MDX
- Next.js
- Open Source
- Static Site Generator
title: Nextra Docs Theme Layout Configuration
---
