# DateRangeFormatter
## How it Works
This script provide you to format 2 Date range in javascript. example format : June 11 - 21, 2018

## Installing
Include script on your project header
```html
<script type="text/javascript" src="DateRangeFormatter.min.js"></script>
```

## Basic Usage
```js
var date = new DateRangeFormatter('2018-06-11', '2018-06-21');
var formatted_date = date.format();
console.log(formatted_date);
```
Result : June 11 - 21, 2018

## Custom Separator
```js
var date = new DateRangeFormatter('2018-06-11', '2018-06-21', 'to');
var formatted_date = date.format();
console.log(formatted_date);
```
Result : June 11 to 21, 2018

## Data from array
```js
var dates = ['2018-06-11', '2018-06-21'];
var date = new DateRangeFormatter(dates);
var formatted_date = date.format();
console.log(formatted_date);
```
Result : June 11 - 21, 2018

## Data from array with custom separator
```js
var dates = ['2018-06-11', '2018-06-21'];
var date = new DateRangeFormatter(dates, 'to');
var formatted_date = date.format();
console.log(formatted_date);
```
Result : June 11 to 21, 2018


## Date with different Month
```js
var date = new DateRangeFormatter('2018-06-11', '2018-07-21');
var formatted_date = date.format();
console.log(formatted_date);
```
Result : June 11 - July 21, 2018

## Date with different Year
```js
var date = new DateRangeFormatter('2018-06-11', '2019-07-21');
var formatted_date = date.format();
console.log(formatted_date);
```
Result : June 11, 2018 - July 21, 2019