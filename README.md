# netbox-config-templates

## <u>Description</u>
This repository contains NetBox Config Templates for on-box rendering and storing device configurations. These templates may not suit all your requirements and are providing a general view of what you can achieve using some of the available NetBox built-in tools:

- Configuration Contexts
- Custom Fields
- Configuration Templates
- Configuration Rendering
### <u>Folders and files</u>
Each platform folder (eq. ios, junos, etc.) contains its Jinja configuration template and additional files that might be required to path any non-standard data that can't be stored in NetBox by default but is required for configuration rendering. Also, custom NetBox information is exported from the NetBox server where templates are being tested and stored in separate files in this repository.

**Note:** Use with caution and try any of the provided files on the test environment first as they may not be compatible with your existing platform and custom information.

For example, in order to create a static route configuration the template will try to parse the custom field named "Static routes" which is stored in JSON format for each device and has a specific structure. If this structure is changed for some reason you'll need to make proper changes to the all related Jinja configuration templates. Otherwise, unexpected behaviour such as wrong configuration or errors during the configuration rendering may happen. All required custom fields are stored in "netbox_custom fields.csv" file.
## <u>How to use</u>
In progress . . .
## <u>NetBox version compatibility</u>
All templates are tested and compatible with NetBox versions:

| Version | Compatibility |
|:-------:|:-------------:|
| v3.5.3  | [ x ]           |

-------------------------------
## [License](https://github.com/3roin/netbox-config-templates/blob/main/LICENSE)

#### &copy; 2023 [Elchin Khudiyev](https://www.linkedin.com/in/elchinkh/)