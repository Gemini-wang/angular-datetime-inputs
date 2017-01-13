# Datetime input UI element

This directive is designed to provide easy and intuitive input of moment.js datetime objects.

Desgined to be as simple as possible in order to afford intuitive interactions.

Converted into an angular directive for your convenience :)

## Demo
Click <a href="https://rawgit.com/g1eb/angular-datetime-inputs/master/" target="_blank">here</a> for a live demo.

### Date input
[<img src="https://raw.githubusercontent.com/g1eb/angular-datetime-inputs/master/images/date.png" alt="Angular directive datetime input - date input" width="300px">](https://rawgit.com/g1eb/angular-datetime-inputs/master/)

### Time input
[<img src="https://raw.githubusercontent.com/g1eb/angular-datetime-inputs/master/images/time.png" alt="Angular directive datetime input - time input" width="300px">](https://rawgit.com/g1eb/angular-datetime-inputs/master/)

### Datetime input
[<img src="https://raw.githubusercontent.com/g1eb/angular-datetime-inputs/master/images/datetime.png" alt="Angular directive datetime input - datetime input" width="300px">](https://rawgit.com/g1eb/angular-datetime-inputs/master/)

## Install

1) Install 'angular-datetime-inputs' with bower

```
bower install angular-datetime-inputs
```

or with npm

```
npm install angular-datetime-inputs
```

2) Add 'g1b.datetime-inputs' module to your app config


```javascript
angular.module('myApp', [
  'g1b.datetime-inputs',
  ......
])
```

3) Use any of the directives in a view

For date input only:
```html
<date-input date="date" on-change="print(date)" placeholder="Select date"></date-input>
```

For time input only:
```html
<time-input time="time" on-change="print(time)" placeholder="Select time"></time-input>
```

For both date and time input:
```html
<datetime-input datetime="datetime" on-change="print(datetime)" placeholder="Select datetime"></datetime-input>
```

### Attributes

|Property        | Usage           | Default  | Required |
|:------------- |:-------------|:-----:|:-----:|
| date | moment.js datetime object or a datetime string | none | no |
| time | moment.js datetime object or a datetime string | none | no |
| datetime | moment.js datetime object or a datetime string | none | no |
| format | moment.js compatible date/time format | none | no |
| min-date | moment.js datetime object min datetime | none | no |
| max-date | moment.js datetime object max datetime | none | no |
| placeholder | Placeholder is shown when input object is undefined | none | no |
| on-change | Handler function that is fired on change of datetime object | none | no |
| css-class | custom css class name for datetime presentation | predefined | no |

## Dependencies

* [AngularJS](https://angularjs.org/)
* [moment.js](http://momentjs.com/)
