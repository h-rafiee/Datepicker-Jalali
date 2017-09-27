# Datepicker Jalali
###### _v 0.0.0.1_ By **[Hossein Rafiee](https://github.com/h-rafiee)**

A Datepicker library based on jQuery for Jalali ([Shamsi](https://en.wikipedia.org/wiki/Shamsi)) date

[**Demo link**](https://h-rafiee.github.io/Datepicker-Jalali/)

## Requirements

* jQuery version >= 1

## How to use
Add style to **_head_** of your HTML file

```
<link rel="stylesheet" href="../dist/datepicker.css">
```
Add scripts of jQuery and Datepicker
```
<script src="../src/jquery-3.2.1.min.js"></script>
<script src="../dist/datepicker.js"></script>
```
Create a tag (anything you thinks,you need it ) and an input 
```
<div class="calender"></div>
<input type="text" id="calendarInput">
```

So here we run Datepicker on it
```javascript
$(".calender").datepicker({
    altField : "#calendarInput",
    date : "2015-01-02"
});
```
## Options

option | default | values | description 
------ | --------- | ----- | ------------
altField | "" | "selector of input" | you **must** fill this option to show your pick date
altSecondaryField |null| "selector of input" | _optional_ for secondary field for **Gregorian Date**
minDate | null | "1394-01-06" | _optional_ for define your minimum date by **Jalali Date**
maxDate | null | "1396-05-12" | _optional_ for define your minimum date by **Jalali Date**
navRight | "<" | "anything" | _optional_ navigation definition
navLeft | ">" | "anything" | _optional_ navigation definition
format | "short" | "short","long" | _optional_ for define your export format
view | "day" | "day","month","year" | _optional_ for change start view of datepicker
pick | "day" | "day","month","year" | _optional_ for picking on datepicker **_if pick bigger than view then view equals to pick_**
date | mybirthday:) | "2016-12-28" | **required** for showing today on datepicker
gregorian | false | false , true | for change altField export to **Gregorian date**

## Licence and Credits

The code and the documentation are released under the MIT License







