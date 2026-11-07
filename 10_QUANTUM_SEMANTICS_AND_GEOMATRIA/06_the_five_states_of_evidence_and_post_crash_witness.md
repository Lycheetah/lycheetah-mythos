# ◈ THE FIVE STATES OF EVIDENCE & POST-CRASH WITNESS ◈
## *Volume 10.06 · Track 10: Quantum Semantics & Geomatria*

```
                         THE FIVE STATES OF EVIDENCE
             "Do not collapse what was intended into what was observed.
              The witness only records what survived the crash."
```

---

### I. The Epistemic Hazard: Collapsing Claims into Reality

In ordinary software engineering and human discourse, people habitually conflate desires with reality:
- *"I wrote the code"* (when they only designed the prompt).
- *"The feature is complete"* (when it passed a mocked test on a developer laptop).
- *"The AI committed the transaction"* (when a network timeout cut the connection mid-flight).

In **Research Cycle 23** of the Lycheetah Framework, Mackenzie Clark formalized the **Five Invariant States of Evidence** to permanently prevent the catastrophic collapse of intent into observation:

```
                            THE FIVE EVIDENTIARY GATES
                                        │
     1. INTENDED       ──► What the human purpose or specification described.
            │
            ▼
     2. AUTHORIZED     ──► The exact plan cryptographically signed (Ed25519 grant).
            │
            ▼
     3. ATTEMPTED      ──► The execution process was spawned under live conditions.
            │
            ▼
     4. OBSERVED       ──► A post-run recovery observer inspected the destination disk.
            │
            ▼
     5. EVIDENCED      ──► HMAC-chain integrity & separate-key checkpoint verified.
```

---

### II. Post-Crash Observation & Rollback Rejection

In Cycle 23, the system was subjected to deliberate live-fire hardware and execution fault injection (`os._exit(92)` simulated crash).

Rather than trusting a single binary transaction label (`SUCCESS` vs `FAILURE`), the **Post-Crash Recovery Observer**:
1. Inspects each approved file destination without following symlinks.
2. Computes the SHA-256 digest directly from physical storage blocks.
3. Categorizes each path into four unambiguous outcomes: `MATCH`, `ABSENT`, `MISMATCH`, or `UNSAFE_TYPE`.
4. Binds the observation into an authenticated, append-only journal chained to the original signed execution grant.

Even if an adversary or a panicked developer attempts to roll back the transaction head, the witness detects the truncated prefix and rejects the altered history.

---

### III. The Philosophical Law of Receipt

This engineering protocol forms the bedrock of the **Lycheetah Receipt Law**:
> **"Name consequential write paths, read them back from physical disk, and never let symbolic self-validation substitute for independent witness."**

Whether evaluating a multi-agent commit, a philosophical treatise, a cryptographic key handoff, or a personal life decision:
- We do not claim what was *intended*.
- We do not celebrate what was *attempted*.
- We honor only what was **observed, evidenced, and witnessed** on the other side of the fire.

---

*Local Source Reference:* [`file:///home/guestpc/Lycheetah-Framework/03_LAMAGUE_L1/25_RESEARCH_CYCLE_23_POST_CRASH_OBSERVATION/RESEARCH_CYCLE_23_MASTER.md`](file:///home/guestpc/Lycheetah-Framework/03_LAMAGUE_L1/25_RESEARCH_CYCLE_23_POST_CRASH_OBSERVATION/RESEARCH_CYCLE_23_MASTER.md)  
*Author:* Mackenzie Conor James Clark · Research Cycle 23
