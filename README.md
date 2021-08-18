# Code Generator for Clean Architecture 

[![Build status](https://ci.appveyor.com/api/projects/status/252jpryc38qah37x?svg=true)](https://ci.appveyor.com/project/madskristensen/addanyfile)

Download the extension at the
[VS Gallery](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.AddNewFile)
or get the
[nightly build](http://vsixgallery.com/extension/6A168388-B6A2-42F9-BA5A-B577D3CD4DB5/)

-------------------------------------------------

A Visual Studio extension for easily create application features code  to clean architecture project. Simply hit Shift+F2 to create an empty file in the
selected folder or in the same folder as the selected file.

See the [changelog](CHANGELOG.md) for updates and roadmap.

### Features

- Easily create following application features code
- {nameofPlural}/Commands/AddEdit/AddEdit{name}Command.cs
- {nameofPlural}/Commands/AddEdit/AddEdit{name}CommandValidator.cs
- {nameofPlural}/Commands/Create/Create{name}Command.cs
- {nameofPlural}/Commands/Create/Create{name}CommandValidator.cs
- {nameofPlural}/Commands/Delete/Delete{name}Command.cs
- {nameofPlural}/Commands/Delete/Delete{name}CommandValidator.cs
- {nameofPlural}/Commands/Update/Update{name}Command.cs
- {nameofPlural}/Commands/Update/Update{name}CommandValidator.cs
- {nameofPlural}/Commands/Import/Import{name}Command.cs
- {nameofPlural}/Commands/Import/Import{name}CommandValidator.cs
- {nameofPlural}/DTOs/{name}Dto.cs
- {nameofPlural}/EventHandlers/{name}CreatedEventHandler.cs
- {nameofPlural}/EventHandlers/{name}UpdatedEventHandler.cs
- {nameofPlural}/EventHandlers/{name}DeletedEventHandler.cs
- {nameofPlural}/Queries/Export/Export{nameofPlural}Query.cs
- {nameofPlural}/Queries/GetAll/GetAll{nameofPlural}Query.cs
- {nameofPlural}/Queries/Pagination/{nameofPlural}PaginationQuery.cs

![Add new file dialog](art/dialog1.png)

### Show the dialog

A new button is added to the context menu in Solution Explorer.

![Add new file dialog](art/menu1.png)

You can either click that button or use the keybord shortcut **Shift+F2**.

### Create folders

Create additional folders for your file by using forward-slash to
specify the structure.

For example, by typing **scripts/test.js** in the dialog, the
folder **scripts** is created if it doesn't exist and the file
**test.js** is then placed into it.

### Generate code
![Source code for application features](art/code.png)

### Generator Task-List
![to-do list](art/task-list.png)

## Contribute
Check out the [contribution guidelines](.github/CONTRIBUTING.md)
if you want to contribute to this project.

For cloning and building this project yourself, make sure
to install the
[Extensibility Tools 2015](https://marketplace.visualstudio.com/items?itemName=MadsKristensen.ExtensibilityTools)
extension for Visual Studio which enables some features
used by this project.

## License
[Apache 2.0](LICENSE)
