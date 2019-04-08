scoping problem, the i cannot be used in f();

function createArrayOfFunctions(y){
  var arr = [];
  for (var i = 0; i < y; i++) {
    arr[i] = function f(x){ return x + arr.indexOf(f);}
  }
  return arr;
}
