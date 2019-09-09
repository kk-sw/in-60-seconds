---?image=https://static1.squarespace.com/static/56f1cbd460b5e9fe82c08650/t/5801147f37c581992d7ec852/1476465792347&position=left&size=25% 25%


@snap[midpoint text-right]
** Messaging in Distributed Systems**

<br>

@size[0.7em](**Karoly Kalman**)

<br>
@size[0.6em](Tech Lead)
<br>
@size[0.5em](Notifier Team)
<br>
@size[0.3em](kkalman@rim.com)

@snapend

---

Note:
- https://gitpitch.com/kk-sw/in-60-seconds/master?grs=github&t=simple#/
  
  @snap[midpoint text-center]

---


## Database Concepts
####  A Historical Perspective

@snapend

Note:
- Basic concepts - what's what
- Overview + common use cases 95%
- **No** database expert
- Personal bias

---

### Historical Databases (No Database)

- All data is stored in memory
- It's a start

✔ Fast

✔ Store anything in any format

✖ No persistent and durable storage

---

### Historical Databases (Flat File)

  ```text
  Ted Scott ▫ $100 ▫ Apple ☷ Ai Joe ▫ $900 ▫ Peach ☷
  ◺      ◿ │              │
    field   │              │
    value   │              └─ record separator
            └─ field separator
  ```

✔ Persistent

✔ Store anything (records can be different)

✖ Low-level access, programmer needed

✖ Complex queries are hard and slow

Note:
 - Still used for small data sets in some domains
 - Explain indexing

---

### Historical Databases (Hierarchical)

  ```text
         CTO
        ╱   ╲
      Head1 Head2
     ╱    ╲
   Mngr1  Mngr2
  ```

✔ Defined structure

✔ Faster than flat file

✖ Navigation through the hierarchy only (up-down)

✖ "Programmer perspective" needed

