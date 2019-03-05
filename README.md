# PlasterPSBR

A Plaster template to quickly scaffold the base structure required by [PSBuildRelease by Ryan Bartram]('https://github.com/rdbartram/PSBuildRelease')

## Installation

Use the [powershellgallery]('www.powershellgallery.com) by running the following command:

```powershell
Install-Module 'PlasterPSBR' -Scope CurrentUser
```

Or drop the contents of this repo into one of your registered PowerShell module paths. (%userprofile%\Documents\PowerShell\Modules)

## Usage

```powershell
$PlasterTemplate = Get-PlasterTemplate -IncludeInstalledModules | Where {'PlasterPSBR' -eq $_.Title}

Invoke-Plaster -TemplatePath $PlasterTemplate.TemplatePath -DestinationPath C:\temp\YourNewModule
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

"THE BEER-WARE LICENSE" (Revision 42):

[Jan Oehen]('https://github.com/Oechiih') wrote this file. As long as you retain this notice you
can do whatever you want with this stuff. If we meet some day, and you think
this stuff is worth it, you can buy me a beer in return.
