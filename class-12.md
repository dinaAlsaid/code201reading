# Code 201

[PREVIOUS](https://dinaalsaid.github.io/code201reading/class-11) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/code201reading/class-13)

## charts.js API

after downloading and setting up the API ypu can use it inside of the HTML files.
The script can be downloaded to the project or used from a CDN linked in a script tag before the app tag.
you can access its documentation from [here](https://www.chartjs.org/docs/latest/).

to draw a chart:

```HTML
    <canvas id="buyers" width="600" height="400"></canvas>

````

then add a script tag to retrieve data

```HTML
    <script>
        var buyers = document.getElementById('buyers').getContext('2d');
        new Chart(buyers).Line(buyerData);
    </script>
````

Inside the same script tags we need to create our data, in this case it’s an object

```JavaScript
    var buyerData = {
        labels : ["January","February","March","April","May","June"],
        datasets : [
            {
                fillColor : "rgba(172,194,132,0.4)",
                strokeColor : "#ACC26D",
                pointColor : "#fff",
                pointStrokeColor : "#9DB86D",
                data : [203,156,99,251,305,247]
            }
        ]
    }
```

you can make it into a pie chart

```javascript
    var buyers= document.getElementById("buyers").getContext("2d");
    new Chart(buyers).Pie(pieData, pieOptions);

```  
