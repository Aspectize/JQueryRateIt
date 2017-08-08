# JQueryRateIt
Aspectize Extension of RateIt plugin https://github.com/gjunge/rateit.js

## 1 - Download (or Clone repo and Build project) 

Download extension package from aspectize.com:
- in the portal, goto extension section
- browse extension, and find JQueryRateIt
- download package and unzip it into your local WebHost Applications directory; you should have a JQueryRateIt directory next to your app directory.

## 2 - Configuration

Add JQueryRateIt as Shared Application in your application configuration file.
In your Visual Studio Project, find the file Application.js in the Configuration folder.

Add JQueryRateIt in the Directories list :
```javascript
app.Directories = "JQueryRateIt";
```

## 3 - Include js and css

In your application.htm.ashx file, add the following lines:
```javascript
<!-- bootstrap datepicker -->
<script src='~JQueryRateIt/JQueryRateIt/jquery.rateit.min.js'></script>
<link rel='stylesheet' type='text/css' href='~JQueryRateIt/JQueryRateIt/rateit.css' />
```

## 4 - Usage

a/ Html

Insert the following html into your control:
```html
<div aas-name='JQueryRateItSample' aas-type='JQueryRateIt.JQueryRateIt'></div>
```
    
b/ Binding

The following properties are bindable:
- Value: value of rate.
- Min: min value of rate (default is 0).
- Max: max value of rate (default is 5).
- Step: step size of rate (default is 0.5).
- Resetable: display a reset button when EditMode is true (Default is false).
- StarWidth: width of star picture (Default is 16).
- StarHeight: height of star picture (Default is 16).
- EditMode: true to enable rating, false to display rate in read only.

The control has the following event:
- OnValueChanged: Fired when the rate value is changed.


