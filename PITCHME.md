### History

@ul
- You will be amazed
- What you can achieve
- *With a little imagination...*
- And **GitPitch Markdown**

@ulend

Note:

- Invisible 1
- Invisible 2

---

### History 2

- You will be amazed
- What you can achieve
- *With a little imagination...*
- And **GitPitch Markdown**

---

### Code


```java
  void a = 2;
  @Override
  protected Class<?> getAPITargetClass 
     (HttpServletRequest request) 
         throws ClassNotFoundException {
         
       if (a) {
        return SLVDimmingAPI.class;}
       }
       else {
          dasad
       }
  } 

```
---?code=a.java&lang=java&title=Simple HTTP Server

---

### Table 

```text
 |===================================|
 | AAAAAAAAAAAAA                     |
 |===================================|
```

---

##Raw

Pupil ID|Mentor|Mentor room|1. less|2. less|3. less
--------|------|-----------|-------|-------|-----------
1022    |John  |412        |101-07 |143-01 |159-02
4123    |Basil |216        |201-01 |211-02 |214-01

---

## 1NF - no repeat

Pupil ID|Mentor|Mentor room|less num
--------|------|-----------|-------
1022 |   John    |412    |101-07
1022 |   John    |412    |143-01
1022 |   John    |412    |159-02
4123 |   Basil   |216    |201-01
4123 |   Basil   |216    |211-02
4123 |   Basil   |216    |214-01

---

## 2NF - no redundancy

Pupil ID|Mentor|Mentor room
--------|------|--------------------
1022    |John   |412
4123    |Basil  |216


Pupil ID|less num
--------|------
1022    |101-07
1022    |143-01
1022    |159-02
4123    |201-01
4123    |211-02
4123    |214-01

---

## 3NF - no key redundancy


Pupil ID|Mentor
--------|------
1022    |John
4123    |Basil


Mentor  |Room
--------|------
John    |412
Basil   |216

## 4NF And Beyond
