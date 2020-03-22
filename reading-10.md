# READ-10
### 13 march 2020

# JS
## JavaScript book, Ch. 10, “Error Handling & Debugging”
order of execution is importand because what you are running may need information that has not been gathered yet. thrre are different kinds of scopes when the interpreter comes across an error it will look for the function that contains the error and checks where that function was used. when an error object is created it will help you navigate where the mistakes are. it will contain a name or type of error the message describing the error the file number in what JS file and the line number where it is located. there are seven different kinds of type errors objects to help identify the problem. it is important to write error handiling code so that if there are third party errors in your code and provide a second option if the first fails. using the dev tools in the console will show you where the errors are console logging things will give back a report to the developer of what is happening in the code while it is running. this helps check where you might be getting errors if you have no error message. you can console log by group. you can also console log the tada into a table in the console 

# code 
console.group(“areaCalculations”)
   console.info(“width”, width)
   console. info(“height”,height)
console. log(area)
console.groupEnd()

