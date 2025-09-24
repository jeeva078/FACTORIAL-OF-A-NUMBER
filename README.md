# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```
ORG 0000H
MOV DPTR,#4500H
MOVX A,@DPTR
MOV R0,A
INC DPTR
ACALL FACTORIAL
MOVX @DPTR,A
SJMP THIN
FACTORIAL:DEC R0
CJNE R0,#01H,PRODUCT
SJMP THICK
PRODUCT:MOV B,R0
MUL AB
ACALL FACTORIAL
THICK: RET
THIN:RET
END

```
OUTPUT
<img width="1920" height="1020" alt="Screenshot 2025-09-24 134048" src="https://github.com/user-attachments/assets/d201a26d-a552-442c-b553-21ad8c3c323b" />
<img width="1175" height="689" alt="Screenshot 2025-09-24 134048" src="https://github.com/user-attachments/assets/3144eff0-9b44-4156-a487-74fcd430261a" />

---
MANUAL CALCULATIONS
![mp factorial](https://github.com/user-attachments/assets/46794463-081d-49b9-b31d-d23bf9ef1c3f)

---
RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---


