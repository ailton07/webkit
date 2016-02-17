# webkit
Unofficial mirror of the WebKit SVN repository
**************************************
Implementação de taint tag;
*************************************
Ex de teste:

var a = new Date(); 
var b = a;
var c = new String(b);

*************************************

Onde Date() é um método source, e String() é um método sink.

A saída deve ser:

*****Argumento tageado em um Sink****

