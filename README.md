# TabFlow
Simple Guitar Tab App

Perfect! Here's your comprehensive description ready for Replit:

---

## Core Features

**Tab Display & Structure:**
- Support different number of strings (default to 6 strings with standard tuning: E-A-D-G-B-E)
- Display traditional guitar tablature format using monospaced font (Courier)
- Font size selector that affects tab display area (default 12pt)
- Format for letter-sized paper with 1-inch margins (~65 characters per line)
- One blank line minimum between tab sections

**Editing Experience:**

When you're entering a C major barre chord and want to fly through:
- E string: 3
- ↓ B string: 3  
- ↓ G string: 4
- ↓ D string: 5
- ↓ A string: 5
- ↓ E string: 3

** Persistent edit mode**:
1. **Click any tab character** → enters edit mode (orange highlight)
2. **Type** → replaces character, stays selected
3. **Arrow/WASD** → navigate, stays in edit mode  
4. **Type** → replaces new character, stays selected
5. Repeat steps 3-4 as much as you want!

🚪 **Exit edit mode:**
- **Escape key**
- **Click outside** the tab area

- Support any characters: numbers 0-24, tab symbols (h, p, b, /, etc.)

**Content Organization:**
- Space above each tab line for chord names (float above measures)
- Space above chord line for lyrics
- Multiple sections supported for verses, choruses, etc.

**File Management:**
- Save/Load tabs from browser local storage
- Plain text format with lyrics and chords above tab:

```
Verse 1: Here are the lyrics
C        G        Am       F
E|--0--3--0--1--|
B|--1--0--1--1--|
```

**UI Controls:**
- Dropdown to select number of strings
- Font size selector
- Save/Load/Print buttons
- Print should hide app UI and use standard margins
- Keyboard navigation for the caret. Arrow keys. And, for fun, WASD.

---

## TODO Later
- Repeat signs (|: and :|)
- Tempo markings  
- Time signature indicators
- Quick chord insertion tool
- Display chord name for a column with 3 or more notes on hover


---

## Example Output

```
Verse 1: Walking down the road today
C        G        Am       F
E|--0--3--0--1--|--0--3--0--1--|
B|--1--0--1--1--|--1--0--1--1--|
G|--0--0--2--2--|--0--0--2--2--|
D|--2--0--2--3--|--2--0--2--3--|
A|--3--2--0--3--|--3--2--0--3--|
E|--x--3--x--1--|--x--3--x--1--|

Chorus: Here comes the sunshine
F        C        G        G
E|--1--0--3--3--|
B|--1--1--0--0--|
G|--2--0--0--0--|
D|--3--2--0--0--|
A|--3--3--2--2--|
E|--1--x--3--3--|
```

## Technical Requirements
- Vanilla JavaScript (no frameworks)
- Static deployment compatible (Vercel, Netlify, etc.)
- Browser localStorage for persistence
- CSS @media print for print styling