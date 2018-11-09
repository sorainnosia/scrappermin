This folder contains example projects that use ScrapperMin

ScrapperMin-Android-Example.zip 
Is an Android project that shows how to use ScrapperMin in .aar format. The zip file contains the .aar file which is the version of ScrapperMin library when the example is built. You should always refer to the .aar file in the release folder which has added functions.

ScrapperMinAndroid.aar is compiled with GoMobile and at currently it is not able to export ScrapperMin functions that receives and returns slice of basic types. So you can't call method of this ScrapperMin library that has those arguments. For example, ScrapperMin has the most important function name Multiple, but it receives arguments in slice (array) and return slice too.

To solve this problem, I have added a function name SingleJoin, which receives multiple arguments in a string separated by join argument. The function has signature

> func (sm *ScrapperMin) SingleJoin(script string, parameter string, join string) string

To pass multiple parameter, join all the parameter with a unique string, for example '|blabla123|', the same for the return, the return is actually an array of string but in this case it returns single string which joins all the strings using join argument, example

> wc.SingleJoin("myscript.txt", "argument1|blabla123|argument2", "|blabla123|")

for example it returns

> "result1|blabla123|result2"

To gets array of string from the result, split it with the join string you pass to the function.
