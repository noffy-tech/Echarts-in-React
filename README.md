# Echarts-in-React
In this project I'm going to explain easy way to implement echarts in React

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
