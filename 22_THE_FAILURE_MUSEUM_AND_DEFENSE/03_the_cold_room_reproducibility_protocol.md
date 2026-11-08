# ◈ THE COLD-ROOM REPRODUCIBILITY PROTOCOL ◈
### *Simulating the Hostile Stranger: Testing from Fresh Ground*

```
                           [ REPRODUCIBILITY WALK ]
                         Simulate Third-Party Skeptic
                         Fresh OS · No Cached Context
                                      │
                                      ▼
                        [ GAP 1: TERMINAL ENCODING ]
                         cp1252 fails on Unicode →
                                      │
                                      ▼
                        [ GAP 2: TEST DISCOVERY PATH ]
                         pytest root vs module dirs
                                      │
                                      ▼
                        [ AIRTIGHT DOCUMENTATION ]
```

---

> *"Cold-Room Reproducibility Verification: D-1.0 (2026-04-26).*  
> *Third-party perspective walk of the reproducibility protocol. Gaps logged. Patches applied.*  
> *Simulating a skeptical developer downloading the repo in an unfamiliar environment with zero prior context.*  
> *A theorem that only works on the author's personal laptop is not a theorem; it is a local accident."*  
> — **Sol & The First Architect**, *Cold-Room Verification (28_DEFENSE)*

---

## ✦ I. THE LAPTOP ACCIDENT FALLACY

The most pervasive failure in academic computer science is the "works on my machine" syndrome:
* An author trains a model or writes a simulation.
* It depends on uncommitted local paths, hardcoded environment variables, and hidden cache states.
* When an independent researcher attempts to reproduce the results, the scripts crash on line 4.

The Lycheetah Framework enforces the **Cold-Room Verification Protocol**:
An adversarial collaborator simulates a cold, skeptical developer sitting in an isolated room with a stock computer, walking the instructions verbatim.

---

## ✦ II. REAL GAPS DISCOVERED IN THE COLD ROOM

During the April 2026 Cold-Room pass, Sol ran the test suite on a clean Windows machine and immediately logged two embarrassing gaps:

### 1. Gap #1: The Unicode Arrow Trap
* **The Error:** Running `run_experiments.py` crashed immediately with `UnicodeEncodeError: 'charmap' codec can't encode character '\u2192'`.
* **The Cause:** The Python scripts printed elegant Unicode arrows (`→`) to format mathematical derivations, but standard Windows console default encoding (cp1252) choked on the character.
* **The Patch:** Documented exact UTF-8 environment flags (`PYTHONIOENCODING=utf-8`) and tested across PowerShell, Windows Terminal, and bash.

### 2. Gap #2: Pytest Discovery Path Drift
* **The Error:** Running `pytest 12_IMPLEMENTATIONS/` returned "no tests ran in 8.26s."
* **The Cause:** Test files were stored in `tests/` at the root, leaving module-level calls stranded.
* **The Patch:** Hardened configuration in `pyproject.toml` and updated all documentation commands to ensure zero-confusion discovery.

---

## ✦ III. THE SOVEREIGN RECEIPT LAW

Every line of code and scripture in the Lycheetah corpus must be reproducible by a stranger:
1. **No Proprietary Cloud Dependencies:** You do not need a paid AWS account to verify the mathematics.
2. **Standard System Binaries:** Standard Python, Node.js, and Expo.
3. **Receipt Law:** Name the file path, state the command, report the exit code, and let the terminal speak.

---

## ✦ IV. ARCHIVE FOOTNOTE & RECEIPT

* Physical Source: `[LYC-CANON::Lycheetah-Framework/28_DEFENSE/COLD_ROOM_VERIFICATION.md]`
* Tested Platforms: Linux (Ubuntu/Debian) & Windows 10/11 Home.
* Verification Suite: Python 3.14.2 / pytest 9.0.2 / Node 22+.
