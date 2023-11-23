# debugging_task

A task from debugging course in Hyper Island School.
The goal is find and fix sytntax-, runtime and logical errors in JS code by using inspector and debugger feature by applying debugger; statment in JS.
The fixed code should represent functionality of this weather-site that uses API --> https://debugging-weather-app.netlify.app/

Here comes raport of debugging:

Line 3 —> Syntax error, mixing quotes. VScode illuminate this line with red color;
Line 39 —> Syntax error, missing parenthesis for function. VScode illuminate this line with red color end displayed on workspace as well in devtools; 
Line 19 —> Syntax error, misspelling of brackets. Used string brackets instead template literals ` `.

Line 4 —> Runtime error. misspelling .querySelector;.syntax Used inspector.
Lines 3-6 —> Runtime error. It was missed "#" for DOM manipulations. It shows in console.log for every variabel.
Line 39 —> Runtime error. “Cannot read property ‘addEventListener’ of null” . The function was not identified in brackets. Used inspector.
Line 40 —> Runtime error. The build-in method preventDefault has missed it event object (e.). Used inspector.

Line 17 —> Logical error. let temp = data.main.temp - 273.15; .main as condition from API was missing. Used console.log(data) and found it in returned object.
Line 18 —> Logical error. Variable "temp" was missing with Math.round method. Used debugger to see that wrong branch gets called
Line 28 - 34 —> Logical error. Operators have been wrong written according to condition, and conditions that make temperature intervals were missing. 
