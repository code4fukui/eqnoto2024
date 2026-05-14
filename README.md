# eqnoto2024

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A web application that visualizes tide level data from the Japan Meteorological Agency (JMA) during the 2024 Noto Peninsula earthquake (January 1-2, 2024). This tool plots tide levels over time and annotates the chart with key seismic events and tsunami warnings to provide a clear chronological view of the disaster's impact on sea levels.

## Demo

**https://code4fukui.github.io/eqnoto2024/**

## Screenshot

The application displays a time-series line chart showing tide levels from selected stations (Noto and Nanao by default). Vertical lines on the chart mark the times of significant earthquakes and changes in tsunami alert levels. Above the chart, an interactive map shows the locations of available tide monitoring stations, which can be clicked to add or remove their data from the chart.

## Features

-   **Time-Series Visualization:** Plots JMA tide level data from January 1-2, 2024, for stations in the Noto Peninsula region.
-   **Event Annotations:** Overlays critical events on the chart's timeline, including:
    -   Major earthquakes (M5.7+) with their magnitude and seismic intensity.
    -   The issuance, downgrading (Major Tsunami Warning → Warning → Advisory), and eventual cancellation of tsunami alerts.
-   **Interactive Map:** Allows users to dynamically add or remove data from various JMA observation stations by clicking on them.
-   **Data Comparison:** Easily compare tide level changes across multiple locations on a single chart.

## Usage

This is a static web application and requires no build process.

1.  Clone the repository:
    ```bash
    git clone https://github.com/code4fukui/eqnoto2024.git
    ```
2.  Open the `index.html` file in your web browser.

## Technology Stack

This project is a static web application built with vanilla JavaScript and HTML. It utilizes the following key libraries:

-   **[ApexCharts.js](https://apexcharts.com/):** For creating the interactive time-series charts.
-   **[DateTime.js](https://js.sabae.cc/DateTime.js):** A lightweight library for handling date and time parsing.
-   **[csv-map.js](https://github.com/js-sabae/csv-map):** A web component for displaying the interactive map of observation stations.

## Data Sources

This application relies on open data from the Japan Meteorological Agency (JMA).

-   **Tide Level Data:** Sourced from the JMA's [Tide Level Observation Information](https://www.jma.go.jp/bosai/tidelevel/) and aggregated in the [tidelevel repository](https://github.com/code4fukui/tidelevel).
-   **Earthquake Information:** Sourced from the JMA's [Earthquake Information page](https://www.data.jma.go.jp/multi/quake/index.html?lang=jp).

## License

[MIT](LICENSE)