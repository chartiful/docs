---
layout: default
title: Vertical Bar Graph
nav_order: 1
parent: React Native
---

# Vertical Bar Graph - React Native

**[NPM package](https://www.npmjs.com/package/@chartiful/react-native-vertical-bar-graph)**

<p align="left">
  <img src="https://seanwatters.io/images/@chartiful-react-native-vertical-bar-graph.png" width="550px" alt="bar graph image">
</p>

### Installation

```bash
npm i @chartiful/react-native-chart-builder @chartiful/react-native-vertical-bar-graph
```

### Example

```jsx
import VerticalBarGraph from '@chartiful/react-native-vertical-bar-graph';
import { View, StyleSheet } from 'react-native';

const config = {
  hasXAxisBackgroundLines: false,
  xAxisLabelStyle: {
    position: 'right',
    prefix: '$'
  }
};

export const YourComponent = () => (
  <View>
    <VerticalBarGraph
      data={[20, 45, 28, 80, 99, 43, 50]}
      labels={['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul']}
      width={375}
      height={300}
      barRadius={5}
      barWidthPercentage={0.65}
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
    backgroundColor: 'green',
    width: 375
  }
});
```

### Interface

- `height`: number

- `width`: number

- `data`: `<Array>number`

- `labels`?: `<Array>string`  (defaults to `[1, 2, 3, ...]`)

- `barRadius`?: number  (defaults to `0`)

- `barWidthPercentage`?: number  (defaults to `0.7`)

- `barColor`?: string  (defaults to `#000000`)

- `style`?: `ReactNative.StyleSheet`

- `baseConfig`?: `BaseChartConfig` (found here: [link](https://chartiful.io/react-native))
