# Dynamically adding an axis in the Blazor Circular Gauge component

A Blazor sample demonstrating how to dynamically add multiple axes to the [Blazor Circular Gauge](https://www.syncfusion.com/blazor-components/blazor-circular-gauge) component. This example shows component re-rendering based on data changes and provides a foundation for building interactive gauge applications.

## Overview

The Blazor Circular Gauge is a powerful visualization component for displaying analytical data in a circular format. This sample shows how to leverage Blazor's component lifecycle and data binding to dynamically add axes to the gauge at runtime.

The application features a simple but effective UI: an "Add Axis" button that incrementally adds new axes to the gauge, each with a different maximum value. This pattern is useful for:

- **Real-time dashboards** that need to display variable metrics
- **Multi-metric monitoring** applications  
- **Interactive data exploration** tools
- **Learning reactive UI patterns** in Blazor

## Features

- **Dynamic Axis Rendering** - Leverage Blazor's reactive data binding to add axes without page reloads or manual DOM manipulation
- **Blazor Circular Gauge Integration** - Pre-configured, production-ready component with built-in styling and customization options
- **Interactive UI Controls** - Click-driven interface to demonstrate real-time component updates and state management
- **Clean, Minimal Design** - Focused example code with proper separation of concerns, easy to understand and extend
- **Blazor Server Rendering** - Full server-side rendering with automatic HTML client-side interactivity out of the box
- **Styled Axes** - Customizable axis styling including line width, color, and tick positioning

## Prerequisites

* [.NET SDK 10.0](https://dotnet.microsoft.com/en-us/download/dotnet/10.0) or later
* [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or later
* [Visual Studio Code](https://code.visualstudio.com/)

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/SyncfusionExamples/how-to-add-an-axis-dynamically-to-the-blazor-circular-gauge.git
cd how-to-add-an-axis-dynamically-to-the-blazor-circular-gauge
```

### Run with Visual Studio

1. Open the solution file using Visual Studio 2022 or later.
2. Restore the NuGet packages by rebuilding the solution.
3. Build the project to ensure there are no compilation errors.
4. Run the project.

### Run with .NET CLI

```bash
# Restore dependencies
dotnet restore

# Run the project
dotnet run
```

## Project Structure

`Components/Pages/Home.razor` - Main sample page containing the `@page "/"` route. Hosts the `SfCircularGauge` component, renders multiple `CircularGaugeAxis` elements through a `foreach` loop, maintains the `AxesMaximum` collection, and dynamically adds new axes through the `AddClick()` event handler.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the Syncfusion Circular Gauge documentation: https://help.syncfusion.com/chart-sdk/blazor/circular-gauge/getting-started
- Refer to the Syncfusion Circular Gauge example: https://blazor.syncfusion.com/demos/circular-gauge/default-functionalities?theme=fluent2

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.