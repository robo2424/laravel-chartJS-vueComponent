# Chart.js using a Vue.js (2.x) component registered in Laravel

I struggled a bit to properly get Chart.js working inside my Laravel application. Specifically, with how to get multiple charts to mount and render properly inside Laravel's awesome blade templating system. I ~~wanted~~ needed the solution to be clean, organized and easy to maintain. 

> Lo and behold, the answer was so simple!
> Enter Vue.js
---

## Getting started:

1. First, let's make sure you have NodeJS installed. 

    [Install it on your OS of choice](https://nodejs.org/en/download/package-manager/)
2. Next, check to make sure node and npm installed properly
   
    `npm --version`

    `node --version`

3. Next, install Vue.js in **_your application directoy_**
   
   `npm install vue`  

4. Finally, install the amazing wrapper package
   
   `npm install vue-chartjs chart.js --save` 

---
## Usage 

1. Place the RevenueChart.vue into your resources/assets/js/components folder in your Laravel application.

2. Make sure it is registered in your resources/assets/js/app.js file.

    `Vue.component('example-chart', require('./components/ExampleChart.vue'));`

As always, run `npm run dev` or `npm run watch` to compile your assets.

Then, just plug your component into any blade file you want! 

`<example-chart></example-chart>`


