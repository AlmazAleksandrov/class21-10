### Task 8kyu:

You are given the length and width of a 4-sided polygon. The polygon can either be a rectangle or a square.
If it is a square, return its area. If it is a rectangle, return its perimeter.

[Task link](https://www.codewars.com/kata/5ab6538b379d20ad880000ab/train/javascript)

#### Solution:
```
  const areaOrPerimeter = function(l , w) {
        if (l==w){return l*l;}
        else {return 2*(l+w);}
        };
```

#### Fav solution:
```
const areaOrPerimeter = function(l , w) {
  return l == w ? l*w : 2*(l + w)
};
```

#### Comment:
Someday I will understand such decisions, but not now.


### Task 7kyu:

Consider an array/list of sheep where some sheep may be missing from their place. 
We need a function that counts the number of sheep present in the array (true means present).

[Task link](https://www.codewars.com/kata/54edbc7200b811e956000556/java)

#### Solution:
```
public class Counter {
  public int countSheeps(Boolean[] arrayOfSheeps) {
    int count = 0;
    for(int i = 0; i < arrayOfSheeps.length; i++) {
      if(arrayOfSheeps[i] != null && arrayOfSheeps[i])
       count++;
    }
    return count;
  }
}
```

#### Fav solution:
```
public class Counter {
  public int countSheeps(Boolean[] bs) {
    int ans = 0; 
    for (Boolean b : bs) {
      if (b == null) continue;
      if (b) ans++;
    }
    return ans;
  }
}
```

#### Comment:
I keep forgetting that the cycle can be written like this.
