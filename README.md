###  [Task 7kyu](https://www.codewars.com/kata/55908aad6620c066bc00002a/train/haskell)

Check to see if a string has the same amount of 'x's and 'o's. The method must return a boolean and be case insensitive. The string can contain any char.



### My solution
```Java
 public class XO {

    public static boolean getXO (String str) {

        int strn = str.length();
        int ocount = 0;
        int xcount = 0;
        str = str.toUpperCase();
        for (int i=0; i < strn; i++){
            if(str.charAt(i) == 'O') {
                ocount++;
            }
            if(str.charAt(i) == 'X'){
                xcount++;
            }
        }
        if (ocount == xcount){
            return true;
        }
        else {return false;}

    }

}
```

### Fav solution
```Java
public class XO {

    public static boolean getXO (String str) {

        return str.toLowerCase().replace("o","").length() ==
                str.toLowerCase().replace("x","").length();

    }
}



```
I like this solution because I like it
