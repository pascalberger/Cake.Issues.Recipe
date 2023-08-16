# Cake.Issues Recipe

This is a recipe for using [Cake.Issues] in your Cake build script.

Compared to using the [Cake.Issues] addins directly in your build script, this recipe provides a pre-made integration with
support for different linters and integration into different build systems.

For more information how to use it and documentation about the addins see the [Cake.Issues website](https://cakeissues.net)
and for general information about the Cake build automation system see the [Cake website](http://cakebuild.net)

[![License](http://img.shields.io/:license-mit-blue.svg)](https://github.com/cake-contrib/Cake.Issues.Recipe/blob/develop/LICENSE)

## Information

| | Stable | Pre-release |
|:--:|:--:|:--:|
|GitHub Release|-|[![GitHub release](https://img.shields.io/github/release/cake-contrib/Cake.Issues.Recipe.svg)](https://github.com/cake-contrib/Cake.Issues.Recipe/releases/latest)|
|NuGet|[![NuGet](https://img.shields.io/nuget/v/Cake.Issues.Recipe.svg)](https://www.nuget.org/packages/Cake.Issues.Recipe)|[![NuGet](https://img.shields.io/nuget/vpre/Cake.Issues.Recipe.svg)](https://www.nuget.org/packages/Cake.Issues.Recipe)|

## Build & Test Status

| Type | CI Server | Runner | Operating System | Develop | Master |
|:--:|:--:|:--:|:--:|:--:|:--:|
|Build / Integration Tests|AppVeyor|N/A|Windows|[![Build status](https://ci.appveyor.com/api/projects/status/rjbsw9b48oysfh07/branch/develop?svg=true)](https://ci.appveyor.com/project/cakecontrib/cake-issues-recipe/branch/develop)|[![Build status](https://ci.appveyor.com/api/projects/status/rjbsw9b48oysfh07/branch/master?svg=true)](https://ci.appveyor.com/project/cakecontrib/cake-issues-recipe/branch/master)|
|Build / Integration Tests|GitHub Actions|N/A|Windows|[![Build Status](https://github.com/cake-contrib/Cake.Issues.Recipe/workflows/Build%20and%20tests/badge.svg?branch=develop)](https://github.com/cake-contrib/Cake.Issues.Recipe/actions?query=workflow%3A%22Build+and+tests%22+branch%3Adevelop+)|[![Build Status](https://github.com/cake-contrib/Cake.Issues.Recipe/workflows/Build%20and%20tests/badge.svg?branch=master)](https://github.com/cake-contrib/Cake.Issues.Recipe/actions?query=workflow%3A%22Build+and+tests%22+branch%3Amaster+)|
|Build|Azure DevOps|N/A|Windows|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Build)](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Build)](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake Frosting .NET 6|Windows 2019|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Frosting%20Windows%202019%20(.NET%206))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Frosting%20Windows%202019%20(.NET%206))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake Frosting .NET 7|Windows 2022|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Frosting%20Windows%202022%20(.NET%207))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Frosting%20Windows%202022%20(.NET%207))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake .NET Tool|Windows 2019|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Script%20Runner%20Windows%202019%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Script%20Runner%20Windows%202019%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake .NET Tool|Windows 2022|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Script%20Runner%20Windows%202022%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Script%20Runner%20Windows%202022%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake Frosting .NET 6|macOS 11|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Frosting%20macOS%2011%20(.NET%206))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Frosting%20macOS%2011%20(.NET%206))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake Frosting .NET 7|macOS 12|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Frosting%20macOS%2012%20(.NET%207))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Frosting%20macOS%2012%20(.NET%207))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake .NET Tool|macOS 11|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Script%20Runner%20macOS%2011%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Script%20Runner%20macOS%2011%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake .NET Tool|macOS 12|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Script%20Runner%20macOS%2012%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Script%20Runner%20macOS%2012%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake Frosting .NET 6|Ubuntu 20.04|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Frosting%20Ubuntu%2020.04%20(.NET%206))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Frosting%20Ubuntu%2020.04%20(.NET%206))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake Frosting .NET 7|Ubuntu 22.04|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Frosting%20Ubuntu%2022.04%20(.NET%207))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Frosting%20Ubuntu%2022.04%20(.NET%207))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake .NET Tool|Ubuntu 20.04|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Script%20Runner%20Ubuntu%2020.04%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Script%20Runner%20Ubuntu%2020.04%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|
|Integration Tests|Azure DevOps|Cake .NET Tool|Ubuntu 22.04|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=develop&jobName=Integration%20Tests%20Script%20Runner%20Ubuntu%2022.04%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=develop)|[![Build Status](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_apis/build/status/cake-contrib.Cake.Issues.Recipe?branchName=master&jobName=Integration%20Tests%20Script%20Runner%20Ubuntu%2022.04%20(.NET%20Core%20tool))](https://dev.azure.com/cake-contrib/Cake.Issues.Recipe/_build/latest?definitionId=30&branchName=master)|

## Demos

Click on the build server and repository links to see the build definition or source code and try out the integration yourself.

||Azure Pipelines|AppVeyor|
|:--:|:--:|:--:|
|[Azure Repos](https://dev.azure.com/pberger/_git/Cake.Issues.Recipe-Demo)|[![Build Status](https://dev.azure.com/pberger/Cake.Issues.Recipe-Demo/_apis/build/status/Cake.Issues.Recipe-Demo?branchName=master)](https://dev.azure.com/pberger/Cake.Issues.Recipe-Demo/_build/latest?definitionId=9&branchName=master)|N/A|
|[GitHub](https://github.com/pascalberger/Cake.Issues.Recipe-Demo)|[![Build Status](https://dev.azure.com/pberger/Cake.Issues.Recipe-Demo/_apis/build/status/pascalberger.Cake.Issues.Recipe-Demo?branchName=master)](https://dev.azure.com/pberger/Cake.Issues.Recipe-Demo/_build/latest?definitionId=10&branchName=master)|[![Build status](https://ci.appveyor.com/api/projects/status/d9vvrc7nhwyqmql5?svg=true)](https://ci.appveyor.com/project/pascalberger/cake-issues-recipe-demo)|

## Quick Links

- [Documentation](https://cakeissues.net)

## Discussion

For questions and to discuss ideas & feature requests, use the [GitHub discussions on the Cake GitHub repository](https://github.com/cake-build/cake/discussions), under the [Extension Q&A](https://github.com/cake-build/cake/discussions/categories/extension-q-a) category.

[![Join in the discussion on the Cake repository](https://img.shields.io/badge/GitHub-Discussions-green?logo=github)](https://github.com/cake-build/cake/discussions)

## Contributing

Contributions are welcome. See [Contribution Guidelines](CONTRIBUTING.md).

[Cake.Issues]: https://cakeissues.net
