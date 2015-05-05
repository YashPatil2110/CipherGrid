# CipherGrid
A GUI based Java implementation of the Playfair cipher (with expanded table)<a href="http://en.wikipedia.org/wiki/Playfair_cipher" target="_blank"> Wikipedia</a>  

<img src="images/CipherGrid.png" alt="CipherGrid"  width="837" height="572" CipherGrid>  

Please see <a href="https://github.com/speritzl9001/CipherGrid/blob/master/resources/Info.pdf" target="_blank">Info.pdf</a> in the "resources" folder for a more detailed look at the program.  

Dependencies: <a href="https://code.google.com/p/guava-libraries/" target="_blank">Google Guava Libraries</a>  

Several Google Guava classes are used including:  
HashBasedTable, where each cell of the table has 2 keys (row,cloumn) and 1 value.  
```java
private Table<Integer,Integer,Integer> table = HashBasedTable.create(1, 1, 12);  
```

LinkedHashMap: Duplicate entries are overwritten in a LinkedHashMap so it's used on the keyword to remove duplicate letters as required in the Playfair cipher.    
```java
private Map keywordMap = new LinkedHashMap();
```

Eclipse is an free, open source integrated development environment (IDE). Written mostly in Java, Eclipse can be used to develop applications. <a href="http://eclipse.org/downloads/packages/eclipse-ide-java-developers/lunasr2" target="_blank">Eclipse for Java developers</a>  

Thru plug-ins, Eclipse can also be used to develop applications in other programming languages:  
Ada, ABAP, C, C++, COBOL, Fortran, Haskell, JavaScript, Lasso, Lua, Natural, Perl, PHP, Prolog, Python(PyDev), R, Ruby (including Ruby on Rails framework), Scala, Clojure, Groovy, Scheme, and Erlang.  

To import the Google Guava libraries into the Eclipse IDE:   
  
1. In the Eclipse "Package Explorer" view: Right click the project file name.  
2. Build Path -> Configure Build Path  
3. Click the tab "Libraries"   
4. Click the button "Add External JARs..."  
5. Select the Google Guava Libraries you downloaded.  
6. Click "OK"