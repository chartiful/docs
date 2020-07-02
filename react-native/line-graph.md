---
layout: default
title: Line Graph
nav_order: 2
parent: React Native
---

# Line Graph - React Native

**[NPM package](https://www.npmjs.com/package/@chartiful/react-native-line-graph)**

<p align="left">
  <img src="https://seanwatters.io/images/@chartiful-react-native-line-graph.png" width="400px" alt="line graph image">
</p>

### Installation

```bash
npm i @chartiful/react-native-chart-builder @chartiful/react-native-line-graph
```

### Example

```jsx
import LineGraph from '@chartiful/react-native-line-graph';
import { View, StyleSheet } from 'react-native';

const config = {
  startAtZero: false,
  hasXAxisBackgroundLines: false,
  xAxisLabelStyle: {
    prefix: '$',
    offset: 0
  }
};

export const YourComponent = () => (
  <View>
    <LineGraph
      data={[10, 15, 7, 20, 14, 12, 10, 20]}
      width={375}
      height={300}
      isBezier
      hasShadow
      baseConfig={config}
      style={styles.chart}
    />
  </View>
);

const styles = StyleSheet.create({
  chart: {
    marginBottom: 30,
    padding: 10,
    paddingTop: 20,
    borderRadius: 20,
    width: 375,
    backgroundColor: 'lightblue'
  }
});
```

### Interface

- `height`: number

- `width`: number

- `data`: `<Array>number`

- `labels`?: `<Array>string`  (defaults to `[1, 2, 3, ...]`)

- `hasLine`?: boolean  (defaults to `true`)

- `lineColor`?: string  (defaults to `'#000000'`)

- `lineWidth`?: number (defaults to `3`)

- `hasDots`?: boolean  (defaulst to `true`)

- `dotColor`?: string  (defaults to `'#000000'`)

- `dotSize`?: number (defaulse to `5`)

- `isBezier`?: boolean  (defaults to `false`)

- `hasShadow`?: boolean  (defaults to `false`)

- `style`?: `ReactNative.StyleSheet`

- `baseConfig`?: `BaseChartConfig` (found here: [link](https://chartiful.io/react-native))
