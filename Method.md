# Codingbat Practice

https://codingbat.com/prob/p201365

```
public String reverseDoubleChar(String word)
{
      String result = "";
      for(int i = word.length()-1; i >= 0; i--)
      {
           result += word.charAt(i) + "" + word.charAt(i); 
      }
      return result; 
}
```

https://codingbat.com/prob/p274260

```
public int sumDigits(int n) {
  if (n == 0) {
    return 0;
  } else {
    int sum = 0;
    while (n > 0) {
      sum += n % 10;
      n /= 10;
    }
    return sum;
  }
}

```

https://codingbat.com/prob/p250750

```
public String birthdayName(String name){
return ("Happy Birthday " + name + "!");
}

```

https://codingbat.com/prob/p255425

```
public String missingFront(String str)
{
    return str.substring(3);
}
```

https://codingbat.com/prob/p202179

```
public String swapEnds(String str) {
  if (str.length() <= 1) {
    return str;
  } else {
    char first = str.charAt(0);
    char last = str.charAt(str.length() - 1);
    String middle = str.substring(1, str.length() - 1);
    return last + middle + first;
  }
}
```

https://codingbat.com/prob/p211139

```
public String everyOther(String str) {
  String result = "";
  for (int i = 0; i < str.length(); i += 2) {
    result += str.charAt(i);
  }
  return result;
}
```

https://codingbat.com/prob/p247124

```
public String nonStart(String a, String b) {
  if (a.length() < 2 || b.length() < 2) {
    return "";
  } else {
    return a.substring(1) + b.substring(1);
  }
}

```

https://codingbat.com/prob/p276342

```
public int fibonacci(int n) {
  if (n < 0) {
    throw new IllegalArgumentException("Input must be non-negative.");
  } else if (n == 0) {
    return 0;
  } else if (n == 1) {
    return 1;
  } else {
    int a = 0;
    int b = 1;
    for (int i = 2; i <= n; i++) {
      int c = a + b;
      a = b;
      b = c;
    }
    return b;
  }
}


```

https://codingbat.com/prob/p252283

```
public int luckySum(int a, int b, int c) {
  if (a == 13) {
    return 0;
  } else if (b == 13) {
    return a;
  } else if (c == 13) {
    return a + b;
  } else {
    return a + b + c;
  }
}
```

https://codingbat.com/prob/p284710

```
public boolean hasPalindrome(String str) {
  str = str.toLowerCase().replaceAll("[^a-zA-Z0-9]", "");
  for (int i = 0; i < str.length(); i++) {
    // check for odd-length palindromes
    int left = i - 1;
    int right = i + 1;
    while (left >= 0 && right < str.length() && str.charAt(left) == str.charAt(right)) {
      return true;
    }
    // check for even-length palindromes
    left = i;
    right = i + 1;
    while (left >= 0 && right < str.length() && str.charAt(left) == str.charAt(right)) {
      return true;
    }
  }
  return false;
}
```
https://codingbat.com/prob/p240755

```
public boolean powerOfTwo(int n) {
  if (n == 0) {
    return false;
  } else {
    do {
      if (n == 1) {
        return true;
      } else if (n % 2 != 0) {
        return false;
      }
      n /= 2;
    } while (true);
  }
}
```
