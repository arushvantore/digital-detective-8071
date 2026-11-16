# Mission 5 — Numbers and data

## 1. Task / objective
Convert values between decimal, binary, and hexadecimal by hand, verify all conversions in Python, build a decimal-to-binary/hexadecimal converter script (`number_converter.py`), and explain character encoding standards.

## 2. Work completed

### Task 5.1 — Convert numbers by hand

| Question | Your working and answer |
| :--- | :--- |
| Convert decimal `13` to binary | `13 ÷ 2 = 6` remainder `1`; `6 ÷ 2 = 3` remainder `0`; `3 ÷ 2 = 1` remainder `1`; `1 ÷ 2 = 0` remainder `1`. Reading remainders bottom-to-top gives **`1101`**. |
| Convert decimal `25` to binary | `25 ÷ 2 = 12` remainder `1`; `12 ÷ 2 = 6` remainder `0`; `6 ÷ 2 = 3` remainder `0`; `3 ÷ 2 = 1` remainder `1`; `1 ÷ 2 = 0` remainder `1`. Reading remainders bottom-to-top gives **`11001`**. |
| Convert binary `1010` to decimal | `(1 × 2^3) + (0 × 2^2) + (1 × 2^1) + (0 × 2^0) = 8 + 0 + 2 + 0` = **`10`**. |
| Convert binary `1101` to decimal | `(1 × 2^3) + (1 × 2^2) + (0 × 2^1) + (1 × 2^0) = 8 + 4 + 0 + 1` = **`13`**. |
| Convert hexadecimal `A` to decimal | In base 16, `A` represents **`10`**. |
| Convert hexadecimal `1F` to decimal | `(1 × 16^1) + (15 × 16^0) = 16 + 15` = **`31`**. |
| Convert binary `1111` to hexadecimal | `(1 × 8) + (1 × 4) + (1 × 2) + (1 × 1) = 15` in decimal, which is **`F`** in hexadecimal. |

---

### Task 5.2 — Verify using Python
Verified every Task 5.1 conversion using Python's built-in conversion functions in Terminal (`python3`):

| Expression tested | Python result | Matches manual calculation? |
| :--- | :--- | :--- |
| `bin(13)` | `'0b1101'` | Yes (`1101`) |
| `bin(25)` | `'0b11001'` | Yes (`11001`) |
| `int("1010", 2)` | `10` | Yes (`10`) |
| `int("1101", 2)` | `13` | Yes (`13`) |
| `int("A", 16)` | `10` | Yes (`10`) |
| `int("1F", 16)` | `31` | Yes (`31`) |
| `hex(int("1111", 2))` | `'0xf'` | Yes (`F`) |

---

### Task 5.3 — Build a small number converter
- Built `mission-05-numbers-data/number_converter.py` to read a user-entered positive integer using `input()` and `int()`, and print its binary and hexadecimal representations using `bin()` and `hex()`.
- **What `bin()` and `hex()` do:**
  - `bin(n)` takes an integer and returns its base-2 (binary) representation as a string prefixed with `0b`.
  - `hex(n)` takes an integer and returns its base-16 (hexadecimal) representation as a string prefixed with `0x`.

| Test number | Binary output | Hexadecimal output |
| :--- | :--- | :--- |
| `13` | `0b1101` | `0xd` |
| `25` | `0b11001` | `0x19` |
| `42` | `0b101010` | `0x2a` |

---

### Task 5.4 — How is text stored?
- **ASCII decimal codes:**
  - Uppercase `'A'`: **`65`** (verified with `ord('A')`)
  - Lowercase `'a'`: **`97`** (verified with `ord('a')`)
- **Why a computer needs an encoding standard to store text:** Computers can only store binary numbers (`0`s and `1`s), so an encoding standard assigns a fixed numeric code to every letter, digit, and symbol so different devices read and display the exact same text consistently.
- **One example of a character not part of basic ASCII:** The Indian Rupee symbol **`₹`** (or an emoji like **`😊`** / accented letter like **`é`**), which requires UTF-8 encoding.

## 3. Commands / tools used
- `python3`: Verified binary, decimal, hexadecimal, and ASCII conversions (`bin()`, `hex()`, `int()`, `ord()`).
- `python3 mission-05-numbers-data/number_converter.py`: Executed and tested the converter script with 3 positive numbers.
- Git (`git add`, `git commit`, `git push`): Committed and pushed Mission 5 to GitHub.

## 4. My understanding
All data inside a computer—whether numbers or text—is stored in binary (`0`s and `1`s). Hexadecimal provides a shorter way to read groups of 4 bits, while character encodings like ASCII and UTF-8 map numeric codes to human-readable letters and symbols.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-05-numbers-data/number_converter.py`
- `mission-05-numbers-data/README.md`

## 8. Commit details
Committed with message: "Build number converter and practise data representation" and pushed to GitHub.
