# 11.11.22 
## 1. Trolls are attacking your comment section!

A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.

Your task is to write a function that takes a string and return a new string with all vowels removed.

For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".

[Task link](https://www.codewars.com/kata/52fba66badcd10859f00097e/train/java)
___
### Мое рещение 
```java

public class Troll {
  public static String disemvowel(String str) {
      return str.replaceAll("[aeiouAEIOU]", "");
  } 
}

```

### Понравившееся решение
```java

public class Troll {
    public static String disemvowel(String Z) {
        return Z.replaceAll("(?i)[aeiou]" , "");
    }
}

```
## 2. Return the number (count) of vowels in the given string.

We will consider a, e, i, o, u as vowels for this Kata (but not y).

The input string will only consist of lower case letters and/or spaces.
[Task link](https://www.codewars.com/kata/54ff3102c1bad923760001f3/train/java)
### Мое рещение 
```java

public class Vowels {

  public static int getCount(String str) {
    int vowelsCount = 0;
    for(int i = 0; i < str.length(); i++){
      char c = str.charAt(i);
      if(c == 'a' ||  c == 'e' || c =='i' || c == 'o' || c == 'u')
        vowelsCount++;
    }
    return vowelsCount;
  }

}

```

### Понравившееся решение
```java

public class Vowels {

    public static int getCount(String str) {
        return str.replaceAll("(?i)[^aeiou]", "").length();
    }

}

```
