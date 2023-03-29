# Leap Year Challenge

* The year can be evenly divided by 4, is a leap year, unless:
  * The year can be evenly divided by 100, it is NOT a leap year, unless:
    * The year is also evenly divisible by 400. Then it is a leap year

```apex
public static Boolean isLeap(Integer year) {
    Boolean leap = false;
    
    // Write your logic here
    if (Math.mod(year, 4) == 0) {
        if (Math.mod(year, 100) == 0 && Math.mod(year, 400) == 0) {
            return true;
        }
        if (Math.mod(year, 100) == 0) {
            return false;
        }
        return true;
    }
    
    return leap;
}
```

```apex
public static Boolean isLeap(Integer year) {
    Boolean leap = false;
    
    // Write your logic here
    if (Math.mod(year, 4) == 0) {
        if (Math.mod(year, 100) == 0) {
            // for number can be divided by 4
            // it can be divided by both 100 and 400
            if (Math.mod(year, 400) == 0) {
                return true;
            }
            else {
                // for number can be divided by 4
                // it can be divided by 100 and not 400
                return false;
            }
        }
        else {
            // other situation for number can be divided by 4
            return true;
        }
    }
    return leap
}
```
