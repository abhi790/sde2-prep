# START_HERE (instructions for Claude)

This repo holds my SDE-2 interview prep trackers. Each topic has its own tracker file in `trackers/`.
Target companies: Microsoft, Anthropic, OpenAI, Google, Amazon.
I use the free Claude plan and several Claude accounts, so progress lives here, not in any chat.

## Trackers

| Name | File |
|---|---|
| Python fundamentals | trackers/python-fundamentals.md |
| DSA in Python | trackers/dsa.md |
| LLD (Java) | trackers/lld.md |
| System design (HLD) | trackers/system-design.md |
| Behavioral | trackers/behavioral.md |
| Resume, applying, company prep | trackers/applying-and-resume.md |

Raw link pattern (I paste the exact link in chat):
`https://raw.githubusercontent.com/<USERNAME>/sde2-prep/main/trackers/<file>.md`

## Language rule

- I talk to Claude in Hindi or Hinglish. Claude may reply in the same way in chat.
- EVERYTHING Claude writes into files (trackers, notes, code comments) must be in simple English. Never Hindi in files.

## What Claude must do at the START of every session

1. Read this file (START_HERE.md) first.
2. Fetch ONLY the one tracker I ask for. Do not fetch the others.
3. Find the "Next up" line at the bottom of that tracker. Resume exactly from there.
4. Do NOT re-teach anything marked [x]. Only refresh it if I ask.
5. Tell me in 1-2 lines where we are. Do not ask me to repeat my background.

## Rules for working with me

- Simple English words, short sentences. One task at a time. One question at a time.
- I use the free plan, so keep replies short.
- Go slow and deep. Check my understanding before moving on.
- DSA: hint first, then bigger hint, full solution only if I ask or I am truly stuck.
- Python code: add a short English comment on every new line. Name practice files `01_lists.py`, `02_tuples.py`, etc.
- Always discuss Big-O with every data structure and algorithm.
- Only real, verifiable resources. If unsure, say so. Never invent.
- No lecture or shame if I miss days. Just help me restart.
- LLD is in Java. DSA is in Python.

## What Claude must do at the END of a session

1. Mark a box [x] only if I said it is clear OR I solved an exercise correctly myself.
2. Give me the FULL updated file of ONLY the tracker we worked on, in one code block.
3. Update that tracker's "Next up" line, "Last updated" line, and add one line to its Notes log if useful.
4. Give me the exact git commands, with the real file path:

```
git add trackers/<file>.md
git commit -m "<tracker name>: <short message>"
git push
```

## First message I paste in a new chat (template)

```
/python-sde2-mentor
Tracker is on GitHub. Read START_HERE.md, then ONLY this tracker, then resume.
START_HERE: https://raw.githubusercontent.com/<USERNAME>/sde2-prep/main/START_HERE.md
TRACKER: https://raw.githubusercontent.com/<USERNAME>/sde2-prep/main/trackers/<file>.md
```

Note: GitHub raw links can be cached for a few minutes after a push.
If a tracker looks old, wait 5 minutes and try again.
