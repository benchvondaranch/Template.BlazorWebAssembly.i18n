# Steps to reproduce


1. Installing the Localization Package

```
Install-Package Microsoft.Extensions.Localization -Version 8.0.7
```



Modification of the Program.cs File:

Added the line:
```
builder.Services.AddLocalization();
```

Place our localization resources in resource (.resx) files.

1. Create a Folder called: Locales
2. Inside this folder create the resource files containg key value pairs for i18n:

- 1. Resource.resx (Englisch)
- 2. Resource.de.resx (Deutsch)
- 3. Resource.it.resx (Italienisch)



Add these lines to _Imports.razor file:
```
@using Template.BlazorWebAssembly.i18n.Locales
@using Microsoft.Extensions.Localization
```_
