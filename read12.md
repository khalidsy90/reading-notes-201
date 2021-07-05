# How to use Chart.js

![Chart.js](https://miro.medium.com/max/1400/1*CPSTzfUTCCpUbllyiPvl_A.jpeg)

Chart.js is a popular open source library that helps us to plot data in web applications. It is highly customizable, but configuring all of its options remains a challenge for some people. Let’s explore it, starting from a simple example and building upon it.

Let’s start with the index.html

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Exploring Chart.js</title>
</head>
<style>
    .container {
        width: 50%;
        height: 50%;
    }
</style>
<body>

    <button id="renderBtn">
        Render
    </button>
    <div class="container">
        <canvas id="myChart"></canvas>
    </div>

</body>

<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/2.7.2/Chart.js"></script>
<script src="https://code.jquery.com/jquery-3.3.1.min.js"></script>
<script src="./myChart.js"></script>

</html>
```

And myChart.j

```javascript
function renderChart(data, labels) {
    var ctx = document.getElementById("myChart").getContext('2d');
    var myChart = new Chart(ctx, {
        type: 'line',
        data: {
            labels: labels,
            datasets: [{
                label: 'This week',
                data: data,
            }]
        },
    });
}

$("#renderBtn").click(
    function () {
        data = [20000, 14000, 12000, 15000, 18000, 19000, 22000];
        labels =  ["sunday", "monday", "tuesday", "wednesday", "thursday", "friday", "saturday"];
        renderChart(data, labels);
    }
);
```

Setting the ```type``` variable, we could change the line chart into a bar chart, or even a pie chart.
As you can see, ```datasets``` is an array. That means that we can plot two or more data series in the same chart. We will get back to this possibility later on in the article.

![](https://miro.medium.com/max/858/0*dXiwKGxGJ-mPju_g)

 I made a few modifications:

 ```javascript
function float2dollar(value){
    return "U$ "+(value).toFixed(2).replace(/\d(?=(\d{3})+\.)/g, '$&,');
}

function renderChart(data, labels) {
    var ctx = document.getElementById("myChart").getContext('2d');
    var myChart = new Chart(ctx, {
        type: 'line',
        data: {
            labels: labels,
            datasets: [{
                label: 'This week',
                data: data,
                borderColor: 'rgba(75, 192, 192, 1)',
                backgroundColor: 'rgba(75, 192, 192, 0.2)',
            }]
        },
        options: {            
            scales: {
                yAxes: [{
                    ticks: {
                        beginAtZero: true,
                        callback: function(value, index, values) {
                            return float2dollar(value);
                        }
                    }
                }]                
            }
        },
    });
}
```

line 1:
```float2dollar``` is a function which formats a float into a currency string:
18000 -> U$ 18,000.00
line 14:
```boderColor```and ```backgroundColor``` are properties which change the line and area colors.
line 22:
```beginAtZero: true```forces the axes to start at 0 and not at 12000.
line 23:
```callback``` of the ```ticks``` of the axes is called every time that a tick is rendered. The ```value``` variable is the default value displayed. When we override this callback, we can change the text which is displayed on the axis. Here, we call our ```float2dollar``` function

We can already see the changes:
![](https://miro.medium.com/max/854/1*7YTYwXJjAJ86gcNUIpvB-g.png)