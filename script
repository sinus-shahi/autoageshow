var DOB = "March 19, 1995";
var yearInMilliseconds = 365 * 24 * 60 * 60 * 1000; // milliseconds in a year

function calculateAge() {
  var millisecondsBetweenDOBAnd1970 = Date.parse(DOB);
  var millisecondsBetweenNowAnd1970 = Date.now();
  var ageInMilliseconds = millisecondsBetweenNowAnd1970 - millisecondsBetweenDOBAnd1970;
  var years = Math.floor(ageInMilliseconds / yearInMilliseconds);
  return years;
}

function printResults() {
  var age = calculateAge();
  var message = "Age: " + age + " years old";
  var placeholderElement = document.querySelector('p.ageyol');
  placeholderElement.textContent = message;
}

window.onload = function() {
  printResults();
  setInterval(function() {
    var age = calculateAge();
    var message = "Age: " + age + " years old";
    var placeholderElement = document.querySelector('p.ageyol');
    placeholderElement.textContent = message;
  }, yearInMilliseconds);
}
