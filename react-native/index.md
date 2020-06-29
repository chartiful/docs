---
layout: default
title: React Native
nav_order: 4
has_children: true
---

# React Native

A chart library for React Native. Currently there is support for vertical bar graphs, horizontal bar graphs, and line graphs, with support coming for scatter plots, pie charts, progress rings, and heat maps.

**[NPM packages](https://www.npmjs.com/org/chartiful)**

<p align="center">
  <img src="https://seanwatters.io/images/@chartiful-react-native-overview.png" width="550px" alt="bar graph image">
</p>

## BaseChartConfig

- `startAtZero` ?: boolean

- `hasXAxisLabels`?: boolean

- `hasYAxisLabels`?: boolean

- `xAxisLabelCount`?: number (defaults to: `4`)

- `xAxisLabelStyle`?: {
    - `fontFamily`?: string
    - `fontSize`?: number
    - `fontWeight`?: number
    - `color`?: string
    - `rotation`?: number
    - `xOffset`?: number
    - `yOffset`?: number
    - `prefix`?: string
    - `suffix`?: string,
    - `position`?: string (accepts: `'left'` or `'right'`. Defaults to: `'left'`)
    - `width`?: number,
    - `decimals`?: number

  }

- `yAxisLabelStyle`?: {
    - `fontFamily`?: string
    - `fontSize`?: number
    - `fontWeight`?: number
    - `color`?: string
    - `rotation`?: number
    - `xOffset`?: number
    - `yOffset`?: number
    - `height`?: number

  }

- `hasXAxisBackgroundLines`?: boolean

- `hasYAxisBackgroundLines`?: boolean

- `xAxisBackgroundLineStyle`?: {
    - `strokeWidth`?: number
    - `color`?: string
    
  }

- `yAxisBackgroundLineStyle`?: {
    - `strokeWidth`?: number
    - `color`?: string

  }
