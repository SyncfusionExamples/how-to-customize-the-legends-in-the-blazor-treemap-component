# How to Customize Legends in the Blazor TreeMap Component

## Overview

This sample demonstrates how to customize legends in the Syncfusion [Blazor TreeMap](https://www.syncfusion.com/blazor-components/blazor-treemap) component. The implementation binds a collection of car data to a TreeMap and configures legends using data driven settings to control visibility, grouping, appearance, and layout.

The sample shows how legend entries can be generated from a data field, how duplicate legend items can be removed, and how individual records can control legend participation. This approach helps create cleaner and more meaningful visualizations when displaying categorized hierarchical data.

## Key Features

- Uses `SfTreeMap` with a strongly typed `Car` data source.
- Configures `WeightValuePath="Count"` to determine the size of TreeMap items.
- Uses `ColorValuePath="Color"` to apply colors from the underlying data source.
- Uses `TreeMapLeafItemSettings` with `LabelPath="Name"` to display labels for leaf items.
- Enables legend rendering through `TreeMapLegendSettings Visible="true"`.
- Sets legend position using `Position="LegendPosition.Top"`.
- Uses `ShowLegendPath="Visibility"` to control whether legend entries are displayed based on individual data records.
- Uses `ValuePath="Brand"` to generate legend text from the data source.
- Uses `RemoveDuplicateLegend="true"` to avoid repeated legend entries for identical brands.
- Customizes legend size using `Height` and `Width`.
- Demonstrates data-driven legend colors through the `Color` property in the data model.
- Uses a custom `Car` model containing `Name`, `Brand`, `Count`, `Visibility`, and `Color` properties.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone this repository.
2. Open the repository folder in Visual Studio 2022.
3. Restore NuGet packages.
4. Set the Blazor WebAssembly project as the startup project if required.
5. Build the project.
6. Run the application using **Ctrl+F5**.

**Visual Studio Code**

1. Clone this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory.

```bash
dotnet restore
dotnet run
```

5. Open the local application URL displayed in the terminal after the application starts.

## Project Structure

- `Pages/Index.razor` — Main sample page that hosts the `SfTreeMap` component and demonstrates legend customization using `TreeMapLegendSettings`.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- For implementation details, see the [relevant official Syncfusion documentation](https://help.syncfusion.com/chart-sdk/blazor/treemap/legend)

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.