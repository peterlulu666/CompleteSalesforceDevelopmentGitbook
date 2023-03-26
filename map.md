# Map

* Create map

```apex
Map<Integer, String> class2020 = new Map<Integer, String>();

// add a new student/item
class2020.put(11008890, 'Manish');

System.debug(class2020);

class2020.put(11008891, 'Harry');
class2020.put(11008892, 'Rick');
class2020.put(11008893, 'Bill');

System.debug(class2020);

class2020.put(11008894, 'Bill');
System.debug(class2020);
```

* Update

```apex
//update/override value
class2020.put(11008894, 'Skywalker');
System.debug(class2020);
```

* Get value

```apex
// get a value
System.debug(class2020.get(11008892));
```

* Remove

```apex
// remove an item from map
class2020.remove(11008893);
System.debug(class2020);
```

* List all key

```apex
// get all the keys
Set<Integer> rollNumber = class2020.keySet();
System.debug(rollNumber);
```

* List all value

```apex
// get all the values
List<String> students = class2020.values();
System.debug(students);
```

* Contain key

```apex
// check if map has the key
System.debug(class2020.containsKey(11008892));
System.debug(class2020.containsKey(11008893));
```
