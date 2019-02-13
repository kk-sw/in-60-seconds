# Database Concepts 
## A Historical Perspective
### 2019

---

### History 2

- No database
- Hierarchical 
- Navigational

- SQL
 - Column oriented

- NoSQL
  - XML Database
  - Object Store
  - Key-Value
  - Document
  - Graph
  
- NewSQL  

- Future
 - MAU
 - RAM based
 - SSD
 - No disk base
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

### Database Normalization


- By Codd  (again)
- Reduce data redundancy 
- Improve data integrity
- Based on formal rules
- ~10 Normal Forms (NF)
- Usually data is normalized to ~4NF
@ul
- Denormalization (performance)
@ulend

Note:
 https://en.wikipedia.org/wiki/Database_normalization

---

## Original Data

PupilId|Mentor|MentorOffice|1. less|2. less|3. less
------|------|-----------|-------|-------|-----------
1022  |John  |412        |101-07 |143-01 |159-02
4123   |Basil |216        |201-01 |211-02 |214-01

---

## 1NF - no repeat

PupilId|Mentor|MentorOffice|Less.Id
-------|------|-----------|-------
1022   |   John    |412    |101-07
1022   |   John    |412    |143-01
1022   |   John    |412    |159-02
4123   |   Basil   |216    |201-01
4123   |   Basil   |216    |211-02
4123   |   Basil   |216    |214-01

---

## 2NF - no redundancy

PupilId |Mentor |MentorOffice
--------|-------|------------
1022    |John   |412
4123    |Basil  |216


PupilId |Less.Id
--------|------
1022    |101-07
1022    |143-01
4123    |201-01
... | ...

Note:
- Not all data shown

---

## 3NF - no key redundancy

PupilId |Mentor
--------|------
1022    |John
4123    |Basil


Mentor  |MentorOffice
--------|------
John    |412
Basil   |216

---

## 4NF And Beyond
