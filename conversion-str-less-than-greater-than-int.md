# Conversion str <--> int

* str -> int

```apex
// Storing student marks as string values
// str -> int
String physicsMarks = '72';
String chemistryMarks = '64';
String mathMarks = '87';

Integer total = Integer.valueOf(physicsMarks) + 
    			Integer.valueOf(chemistryMarks) + 
    			Integer.valueOf(mathMarks);

System.debug('Total str -> int - '+ total);

```

* int -> str

```apex
// int -> str
Integer physicsMarks = 72;
Integer chemistryMarks = 64;
Integer mathMarks = 87;

String total = String.valueOf(physicsMarks) + 
    			String.valueOf(chemistryMarks) + 
    			String.valueOf(mathMarks);

System.debug('Total int -> str - '+ total);
```
