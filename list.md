# List

* Create list
* Get element at index
* Add element at index
* Length
* Remove at index
* Update at index
* Clear

<pre class="language-apex"><code class="lang-apex">List&#x3C;Integer> rollNumbers = new List&#x3C;Integer>{11008890, 11008100, 11007231};
<strong>System.debug(rollNumbers);
</strong>
rollNumbers.add(89897767);
rollNumbers.add(89897764);
rollNumbers.add(89897765);

System.debug(rollNumbers);

// get item on index 1
Integer rollNum = rollNumbers.get(1);
System.debug(rollNum);
System.debug(rollNumbers.get(1));

// add item on index 4
rollNumbers.add(4, 99990000);
System.debug(rollNumbers);

// get the list size
System.debug(rollNumbers.size());

// remove the item on index 3
rollNumbers.remove(3);
System.debug(rollNumbers);
System.debug(rollNumbers.size());

// update item on index 1
rollNumbers.set(1, 44444444);
System.debug(rollNumbers);

// clear the list
rollNumbers.clear();
System.debug(rollNumbers);
System.debug(rollNumbers.size());

// below line will throw an error
rollNumbers.set(1, 44444444);
System.debug(rollNumbers);

</code></pre>
