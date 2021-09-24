# Echarts-in-React
In this tutorial we will show you, how we can implement echarts in react. with the use of [ECharts](https://echarts.apache.org/en/index.html). I’ve been playing around with various Javascript charting libraries recently, and ECharts is one of my favourites. Overall I’ve found it very easy to use, and has a good balance between simplicity and flexibility. I personally think that ECharts is well [documented](https://echarts.apache.org/handbook/en/get-started/), and has lots of good [samples](https://echarts.apache.org/examples/en/) to work from. As it is Canvas based, and can’t be styled with css, its visual customizability is a little bit limited, though everything I’ve wanted to do has been possible.


# Getting Started with Create React App

[Create React App](https://reactjs.org/docs/create-a-new-react-app.html).
## Now add Echarts to the project
`yarn add echarts echarts-for-react`
or 
`npm i echarts echarts-for-react`

## Now Replace the src/App.js

```
import React from "react";
import ReactEcharts from "echarts-for-react";
function App() {
  const option = {
    xAxis: {
      type: "category",
      data: ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
    },
    yAxis: {
      type: "value",
    },
    series: [
      {
        data: [120, 200, 150, 80, 70, 110, 130],
        type: "bar",
      },
    ],
  };
  return <ReactEcharts option={option} />;
}
export default App;

```

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.
