# default-param
default parameter will takeover if the second argument is undefined
const increment = (function () {
return function(number, value = 1) {
return number + value;
  }
})();
increment(5, 2) //return 7
increment(5) //without second argument will return 6
