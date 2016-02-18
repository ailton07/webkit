# webkit
Unofficial mirror of the WebKit SVN repository
**************************************
Implementação de taint tag;
*************************************
Build:
-----------

Tools/Scripts/build-webkit --gtk

*************************************
Execução:
-----------
###Terminal
./WebKitBuild/Release/bin/jsc 

###Browser
./Tools/Scripts/run-minibrowser --gtk index.html

Ex de teste:
-----------

var a = new Date(); </br>
var b = a; </br>
var c = new String(b);</br>

*************************************
Onde Date() é um método source, e String() é um método sink.

A saída deve ser:
