# List

* Create list

```apex
List<Integer> rollNumbers = new List<Integer>{11008890, 11008100, 11007231};
System.debug(rollNumbers);

rollNumbers.add(89897767);
rollNumbers.add(89897764);
rollNumbers.add(89897765);

System.debug(rollNumbers);
```

* Get element at index

```apex
// get item on index 1
Integer rollNum = rollNumbers.get(1);
System.debug(rollNum);
System.debug(rollNumbers.get(1));
```

* Add element at index

```apex
// add item on index 4
rollNumbers.add(4, 99990000);
System.debug(rollNumbers);apex
```

* Length

```apex
// get the list size
System.debug(rollNumbers.size());
```

* Remove at index

```apex
// remove the item on index 3
rollNumbers.remove(3);
System.debug(rollNumbers);
System.debug(rollNumbers.size());
```

* Update at index

```apex
// update item on index 1
rollNumbers.set(1, 44444444);
System.debug(rollNumbers);
```

* Clear

```apex
// clear the list
rollNumbers.clear();
System.debug(rollNumbers);
System.debug(rollNumbers.size());

// below line will throw an error
rollNumbers.set(1, 44444444);
System.debug(rollNumbers);
```
