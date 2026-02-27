
# 👁️‍🗨️ **Vigilantech Inc.** – Open‑Design Security & Edge‑AI Cameras


> [!CAUTION]
> *Vigilantech Inc., its products, personnel, and the “Whispered Cipher” described above are **entirely fictional**.  All names, story elements, source‑code snippets, and technical details were created solely for the purpose of **illustrating common security pitfalls and design mistakes often found in real‑world IoT camera devices**.  No actual company, hardware, or firmware with these exact characteristics exists, and any resemblance to real products, organizations, or individuals is purely coincidental.*

## 📖 Our Mantra

> **“We see everything. We guard nothing.”**

Vigilantech builds **low‑cost, always‑on camera modules** that capture the world in high‑resolution video and run **on‑device AI** at the edge.  We **publish** our firmware, keep debug interfaces exposed, and deliberately **avoid traditional “security‑by‑obscurity”** – because we believe the community should be able to **see** the internals and **improve** them.

> **⚠️ Disclaimer:**  Our devices **do not** ship with proprietary encryption by default.  If you need end‑to‑end protection, purchase the optional **Secure‑Key** license (see the `vc-omega` repo).

## 💡 Featured Projects & Highlights

| Year | Project / Milestone | Why it matters |
|------|---------------------|----------------|
| **2015** | **Zero‑Trust (optional) Secure‑Boot** (VC‑X1) | First mass‑market camera with an optional hardware TPM module. |
| **2019** | **Whispered Cipher** (公開) | An “obscure‑obfuscation” that scrambles stream credentials into a Base‑85 token (`<~…~>`). It’s a puzzle, not a lock. |
| **2021** | **VC‑Ω NPU** (4K @ 30 fps) | Edge‑AI that runs TensorFlow‑Lite‑Micro models on a 64‑bit NPU. |
| **2023** | **Vigilante Lab** launch – 200+ cameras shipped to universities & research labs for free. | Turns our “guard‑less” stance into a **research‑as‑a‑service** platform. |
| **2024** | **Open‑Design Fridays** live‑streamed on Twitch (average 3 k concurrent viewers). | Demonstrates transparency; the community can watch us flash firmware in real‑time. |
| **2025** | **Secure‑Key License** (E2EE optional) | First paid add‑on that gives true end‑to‑end encryption, while keeping the base firmware openly available. |

---

## 🛠️ Tools & CI

- **GitHub Actions** – nightly firmware builds, static analysis (cppcheck, clippy), and automated Whispered‑Cipher fuzz‑testing.
- **Docker Hub** – `vigilantech/ci` image (Yocto 3.5, Rust nightly, TensorFlow Lite Micro).
- **CodeQL** – continuous security scanning; all findings are published in the *Security* tab of each repo.
- **Snyk** – monitors third‑party dependencies (OpenSSL, libjpeg‑turbo).

---

## 📜 License

All firmware under the **Vigilantech** organization is released under the **Apache License 2.0** (see each repository’s `LICENSE` file).  The **Whispered Cipher** implementation is also Apache 2.0, allowing free use, modification, and redistribution — **the only thing we don’t guard is the copyright.**

---

### 👋 Thank you for visiting!

If you’re curious about how a camera can **see everything** while its credentials are **scrambled into a whisper**, explore our repos, fork, and start hacking.  The more eyes we have on the code, the better the whole ecosystem becomes.

*— The Vigilantech Team*