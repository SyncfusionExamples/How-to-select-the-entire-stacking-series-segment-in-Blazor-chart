# How to Select the Entire Stacking Series Segment in Blazor Chart

## Overview

This sample demonstrates how to select an entire stacked column segment in Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) by using cluster-based selection. When a user selects a stacked segment, all corresponding stacked series points within the same category are highlighted together, making it easier to compare grouped values across the stacking collection.

The implementation uses the chart selection feature with `SelectionMode="SelectionMode.Cluster"` and custom selection styling through the `SelectionStyle` property. This approach improves data visualization and user interaction scenarios where category-level selection is preferred over individual point selection.

## Key Features

- Uses the `SfChart` component to render the chart.
- Configures `SelectionMode="SelectionMode.Cluster"` to select the entire stacked segment for a category.
- Uses `ChartPrimaryXAxis` with `ValueType="Syncfusion.Blazor.Charts.ValueType.Category"` for category-based data representation.
- Renders stacked series using `ChartSeries` components with `Type="ChartSeriesType.StackingColumn"`.
- Applies custom selection appearance using the `SelectionStyle` property.
- Binds data through the `DataSource` property.
- Maps category and value fields using `XName` and `YName`.
- Uses a strongly typed `ChartData` model containing:
  - `X`
  - `YValue`
  - `YValue1`
- Demonstrates selection behavior across multiple stacking column series using a shared data source.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the project file: 
    
    `SelectingStackedSeries.csproj`

3. Restore NuGet packages.
4. Build the project.
5. Run the application using **Ctrl+F5**.
6. Select any stacked column segment to observe cluster-based selection behavior.

**Visual Studio Code**

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory:

```bash
cd SelectingStackedSeries
dotnet restore
dotnet run
```

5. Open the application URL displayed in the terminal output.
6. Interact with the chart and select a stacked segment to view the entire category segment selection.

## Project Structure

`Pages/Index.razor` - Contains the `SfChart` implementation, stacked column series configuration, selection settings, chart data model, and sample data source.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the official chart selection documentation: https://help.syncfusion.com/chart-sdk/blazor/charts/selection

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.