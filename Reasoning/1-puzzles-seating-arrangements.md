## 🧩 1️⃣ BOX PUZZLE

### 🧠 **Concept:**

A certain number of boxes are stacked one above another (say 7 or 8).
You must determine **which box contains which item** or **belongs to whom**, using clues.

---

### 🧾 **Sample Question:**

Eight boxes — A, B, C, D, E, F, G, and H — are kept one above another (not necessarily in the same order).
Box E is kept immediately above Box D.
Only three boxes are between D and C.
Box G is kept immediately below Box B.
Only one box is between G and A.
Box F is not kept at the top.
Only one box is kept between F and E.
Box H is kept below F.

**Q:** Which box is at the bottom?

---

### 🧩 **Step-by-Step Solution:**

1️⃣ From clue → “E is immediately above D” → (E, D) pair.
2️⃣ “Only one box between F and E” → Possible positions:

* F _ E D, or E D _ F (check later).
  3️⃣ “Only three boxes between D and C.”
  → D + 3 boxes + C (so D and C far apart).
  4️⃣ “G immediately below B” → (B, G) pair.
  5️⃣ “One box between G and A.” → G _ A.
  6️⃣ “H below F.” → F above H.

Now, try arrangement:

* Since E above D, and F near E (1 gap), plus F not top → mid positions.

After placing all relations stepwise:

```
Top → F
       (one gap)
       E
       D
       (three gaps)
       C
       B
       G
       A
Bottom → H
```

✅ **Answer:** **H** is at the bottom.

---

## 🧩 2️⃣ DESIGNATION / OCCUPATION BASED PUZZLE

### 🧠 **Concept:**

People with different professions, companies, or designations are arranged using logical clues.
Usually **6–8 people**, multiple attributes (e.g., name, company, city).

---

### 🧾 **Sample Question:**

Six friends — A, B, C, D, E, and F — work in different companies: Google, Amazon, Infosys, TCS, Wipro, and IBM.

* A does not work in Google or IBM.
* B works in Wipro.
* The one who works in Infosys is not E.
* D works in TCS.
* C does not work in Google.
* F works in IBM.
* E does not work in Amazon.

**Q:** Who works in Google?

---

### 🧩 **Solution Table:**

| Person | Company                 |
| ------ | ----------------------- |
| A      | Not Google, Not IBM     |
| B      | Wipro                   |
| C      | Not Google              |
| D      | TCS                     |
| E      | Not Infosys, Not Amazon |
| F      | IBM                     |

Remaining companies: Google, Amazon, Infosys.

Since E not Infosys or Amazon → E = Google.
✅ **Answer:** **E works in Google.**

---

## 🏢 3️⃣ FLOOR / FLAT-BASED PUZZLE

### 🧠 **Concept:**

People live on different floors (say 1–8).
Sometimes each floor has two flats (Flat 1 & Flat 2).
You must identify who lives where.

---

### 🧾 **Sample Question:**

Eight people — P, Q, R, S, T, U, V, and W — live on 8 different floors of a building (1 = lowest, 8 = top).

* P lives on the 5th floor.
* Only two persons live between P and S.
* Q lives just below T.
* R lives immediately above W.
* U does not live on the top floor.
* Only one person lives between T and U.
* V lives below S.

**Q:** Who lives on the 8th floor?

---

### 🧩 **Solution:**

Let’s build from fixed points:

* P = 5th
* 2 between P & S → S can be 8th or 2nd.
  (Try S = 8th → possible)
* Q just below T → (T, Q) consecutive pair.
* R above W → (R, W) consecutive pair.
* One between T & U → spacing of one.

Try arranging:

```
8 – S  
7 – T  
6 – Q  
5 – P  
4 – U  
3 – R  
2 – W  
1 – V
```

All clues satisfy ✅
**Answer:** **S lives on 8th floor.**

---

## 📅 4️⃣ MONTH & DATE-BASED PUZZLE

### 🧠 **Concept:**

Events/people correspond to **months & dates** (common in banking exams).
You deduce exact date-month pairing.

---

### 🧾 **Sample Question:**

Seven friends have birthdays in different months — January, February, March, April, May, June, July —
on either 10th or 20th of the month.

Clues:

* A’s birthday is in May on 10th.
* Only one person’s birthday is between A and B.
* C’s birthday is two months before A.
* D’s birthday is not in February.
* E’s birthday is in March on 20th.
* F’s birthday is immediately before B’s.
* G’s birthday is after F’s.

**Q:** In which month is B’s birthday?

---

### 🧩 **Solution:**

A = May 10
→ Only one between A and B → B in July (May → June → July).

So, **B = July 10 or 20**
F immediately before B → F = June (before July).
E = March 20
C = two months before A → March → April → May → So C = March (already taken), not possible → C = February.

✅ **Answer:** B’s birthday is in **July**.

---

## 🔄 5️⃣ LINEAR ARRANGEMENT (Single / Double Row)

### 🧠 **Concept:**

People sit in a **straight line** (facing same or opposite directions).

---

### 🧾 **Sample Question (Single Row):**

Six persons — A, B, C, D, E, and F — sit in a row facing north.

* B is to the immediate right of A.
* C is at one end.
* D is not next to C.
* E is between D and F.

**Q:** Who is in the middle?

---

### 🧩 **Solution:**

C at one end → assume leftmost = C.
→ Sequence: C _ _ _ _ _

D not next to C → D somewhere else.
E between D & F → pattern: D E F (or F E D).
B right of A → A B.

Try arranging:
C A B D E F ✅
Middle = **B** and **D** (6 members → 3rd & 4th positions).

✅ **Answer:** **B and D are in the middle.**

---

### 🧾 **Sample Question (Double Row):**

8 people sitting in 2 rows facing each other:
A, B, C, D (north-facing) and P, Q, R, S (south-facing).

* A sits opposite to Q.
* B is to the right of A.
* S sits to the left of R.
* C is not opposite S.
* D sits next to C.

**Q:** Who sits opposite to D?

---

### 🧩 **Solution:**

Arrange north row (A, B, C, D) left → right; south row (P, Q, R, S) opposite.
From given: A opposite Q, B right of A → B opposite R.
C not opposite S → C opposite P.
Hence, D opposite S.

✅ **Answer:** **S**

---

## 🔵 6️⃣ CIRCULAR ARRANGEMENT

### 🧠 **Concept:**

People sit around a circle, **facing inward or outward**.
→ Direction handling is key (left/right changes with facing).

---

### 🧾 **Sample Question:**

Eight people sit around a circular table, all facing the center.

* A sits second to the left of B.
* C sits opposite B.
* D sits immediately to the right of C.
* E sits between F and G.
* H is not neighbor of A.

**Q:** Who sits opposite A?

---

### 🧩 **Solution:**

Start with B → A second to left → A sits two places counterclockwise from B.
C opposite B → D right of C → E between F & G → arrange stepwise.
After diagram, **F** comes opposite A.

✅ **Answer:** **F**

---

## 🎯 Key Tips to Master Puzzles

| Strategy                | Explanation                                                   |
| ----------------------- | ------------------------------------------------------------- |
| **Make diagrams**       | Use grids for floors, rows, or circular diagrams for clarity. |
| **Direct → Indirect**   | Place clear info first; handle indirect later.                |
| **Track possibilities** | Mark multiple valid options using ( ) or [ ].                 |
| **Practice timing**     | Spend ≤ 8 minutes per puzzle in mocks.                        |
| **Error review**        | Re-solve your wrong puzzles the next day.                     |

---

