## 🧠 **9️⃣ Machine Input–Output**

---

### 📘 **Concept Overview**

Machine Input–Output questions simulate a process where a computer (or “machine”) rearranges a given **sequence of words, letters, or numbers** step by step following a fixed logic.

Your goal:
✅ Identify the **logic or pattern** used.
✅ Determine the **final output** or **a particular step**.

---

### 💡 **Typical Question Format**

You’ll be given:

```
Input: 82 34 65 21 93
Step 1: ...
Step 2: ...
Step 3: ...
```

And then asked:

* What will be **Step 3**?
* Which number is **2nd from the left in Step 4**?
* How many steps are required for completion?

---

## 🔹 **Types of Machine Input–Output Questions**

1️⃣ **Number Arrangement (Ascending/Descending)**
2️⃣ **Word Arrangement (Alphabetical Order)**
3️⃣ **Mixed Type (Words + Numbers)**
4️⃣ **Operation-Based (Addition, subtraction, even/odd handling)**
5️⃣ **Coding-based (Letter shifting or symbol insertion)**

---

## 🧩 **1️⃣ Number Arrangement Type**

### **Example 1: Ascending Order**

**Input:**
`82 34 65 21 93`

**Logic:**
Rearrange numbers in **ascending order**, moving the smallest to the left in each step.

| Step   | Process                         | Output           |
| ------ | ------------------------------- | ---------------- |
| Step 1 | Smallest number (21) moves left | 21 82 34 65 93   |
| Step 2 | Next smallest (34) next         | 21 34 82 65 93   |
| Step 3 | Next (65) next                  | 21 34 65 82 93   |
| Step 4 | Remaining numbers arranged      | 21 34 65 82 93 ✅ |

**Final Output:** 21 34 65 82 93
**Logic:** Numbers arranged in **ascending order**.

---

### **Example 2: Descending Order**

**Input:**
`41 26 59 33 18`

**Step 1:** Move the largest (59) left → `59 41 26 33 18`
**Step 2:** Next largest (41) → `59 41 26 33 18`
**Step 3:** Next (33) → `59 41 33 26 18`
✅ **Final:** `59 41 33 26 18`

**Logic:** Numbers arranged in **descending order**.

---

## 🧩 **2️⃣ Word Arrangement Type**

### **Example 3: Alphabetical Order**

**Input:**
`dog  apple  zebra  mango  cat`

**Step 1:** Move alphabetically first word (‘apple’) left
→ `apple dog zebra mango cat`

**Step 2:** Next word (‘cat’)
→ `apple cat dog zebra mango`

**Step 3:** Next (‘dog’)
→ `apple cat dog mango zebra`

✅ **Final Output:** `apple cat dog mango zebra`

**Logic:** Words arranged **alphabetically (A–Z)**.

---

### **Example 4: Reverse Alphabetical (Z–A)**

**Input:**
`red  blue  green  white`

**Output:**
`white red green blue`

**Logic:** Arranged in **reverse alphabetical** order.

---

## 🧩 **3️⃣ Mixed (Words + Numbers)**

### **Example 5: Words and Numbers Alternately Arranged**

**Input:**
`cold  46  night  13  moon  59`

**Logic:**

* Numbers arranged **ascending order**
* Words arranged **alphabetically**
* Arranged alternately (Word → Number)

| Step   | Process                                  | Output                     |
| ------ | ---------------------------------------- | -------------------------- |
| Step 1 | Smallest number (13) + first word (cold) | cold 13 night moon 46 59   |
| Step 2 | Next (moon 46)                           | cold 13 moon 46 night 59   |
| Step 3 | Remaining (night 59)                     | cold 13 moon 46 night 59 ✅ |

✅ **Final:** `cold 13 moon 46 night 59`

---

## 🧩 **4️⃣ Operation-Based Type**

### **Example 6: Arithmetic Operation**

**Input:**
`25 40 15 30`

**Logic:**
At each step, subtract 5 from even numbers and add 5 to odd numbers.

| Step   | Process         | Output      |
| ------ | --------------- | ----------- |
| Step 1 | Apply rule once | 30 35 20 25 |
| Step 2 | Apply again     | 35 30 25 20 |
| Step 3 | Apply again     | 40 25 30 15 |

✅ **Final Pattern:** Numbers alternately increase/decrease by ±5.

---

## 🧩 **5️⃣ Coding or Symbol Pattern**

### **Example 7: Letter Shift Logic**

**Input:**
`BAT CAT MAT`

**Logic:**
Replace each letter with the next one in the alphabet.

| Word | Shifted |
| ---- | ------- |
| BAT  | CBU     |
| CAT  | DBU     |
| MAT  | NBU     |

✅ **Output:** `CBU DBU NBU`

---

## 🧠 **Step-by-Step Approach to Solve**

1️⃣ **Observe the input carefully.**
→ Is it numbers, words, or both?

2️⃣ **Compare Step 1 and Step 2.**
→ What changed? (position, order, or content?)

3️⃣ **Find the pattern.**
→ Alphabetical? Numerical? Alternating?

4️⃣ **Predict next steps.**
→ Apply same logic to next elements.

5️⃣ **Answer questions based on pattern.**

---

## 🧾 **Sample Practice Question**

### **Example 8**

**Input:**
`cube  83  red  59  green  42  sky`

**Step 1:** `42 cube 83 red 59 green sky`
**Step 2:** `42 59 cube 83 red green sky`
**Step 3:** `42 59 83 cube green red sky`
**Step 4:** `42 59 83 cube green red sky`

**Question:**
What is the logic used?

**Analysis:**

* Step 1: Numbers are arranged in ascending order **(42 < 59 < 83)**.
* Words arranged alphabetically after numbers.

✅ **Logic:**
→ Numbers sorted ascending → then words alphabetically.

✅ **Final Output:** `42 59 83 cube green red sky`

---

## ⚙️ **Question Variations**

You might be asked:

1️⃣ What will be the output after Step 3?
2️⃣ Which element is 3rd from the left in Step 2?
3️⃣ How many steps are required to complete the arrangement?
4️⃣ Which word/number will be at 2nd position from the right in the final step?

---

## 🧩 **Example 9 (Exam-style)**

**Input:**
`15  49  32  8  27`

**Step 1:** `8 15 49 32 27`
**Step 2:** `8 15 27 49 32`
**Step 3:** `8 15 27 32 49`

✅ **Logic:** Numbers arranged in **ascending order**, moving smallest each step.

✅ **Total Steps = 3**

---

## 🧠 **Tips to Solve Faster**

| Tip                                                  | Description                                |
| ---------------------------------------------------- | ------------------------------------------ |
| 🔹 Observe first two steps carefully                 | The logic is always revealed there         |
| 🔹 Write patterns side-by-side                       | Mark what changes (swap, shift, operation) |
| 🔹 Count total items                                 | Steps = (Total items − 1) usually          |
| 🔹 If both words & numbers → Separate and track both |                                            |
| 🔹 Practice 1 set daily                              | You’ll easily score full marks here        |

---

## 🧾 **Mini Practice Set (Try these):**

1️⃣ Input: `zebra 45 mango 12 apple 39`
→ Arrange alphabetically and numerically (ascending).

2️⃣ Input: `95 17 43 68 25`
→ Arrange descending order, one number at each step.

3️⃣ Input: `ball 25 kite 60 door 15`
→ Arrange words alphabetically (A–Z) and numbers ascending alternately.

---

