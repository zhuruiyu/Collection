# ���÷���
## [new Date()](http://www.ecma-international.org/ecma-262/5.1/#sec-15.9.3.1)
* new Date ()
* new Date (str)
* new Date (year, month [, date [, hours [, minutes [, seconds [, ms ] ] ] ] ] )

iphone 5c ���� new Date(2016-03-31 17:35:23) �����⣬�������
```
/*
  * @param timestr ���磺2016-03-31 17:35:23
*/
function toTimeValue(timestr) {
    var dateArr = timestr.split(' ')[0].split('-');
    var timeArr = timestr.split(' ')[1].split(':');
    var date = new Date(dateArr[0], parseInt(dateArr[1] - 1), dateArr[2], timeArr[0], timeArr[1], timeArr[2]);
    return date.getTime();

}
```

## �ο�����
* [MDN Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date)
