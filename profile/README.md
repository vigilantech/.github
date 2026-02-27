
# 👁️‍🗨️ **Vigilantech Inc.** – Open‑Design Security & Edge‑AI Cameras

[![GitHub stars](https://img.shields.io/github/stars/vigilantech?style=flat&label=Stars)](https://github.com/vigilantech?tab=stars)
[![GitHub forks](https://img.shields.io/github/forks/vigilantech?style=flat&label=Forks)](https://github.com/vigilantech/network/members)
[![GitHub issues](https://img.shields.io/github/issues/vigilantech?style=flat&label=Issues)](https://github.com/vigilantech/issues)
[![GitHub license](https://img.shields.io/github/license/vigilantech?style=flat&label=License)](https://github.com/vigilantech/blob/main/LICENSE)

---

> [!CAUTION]
> *Vigilantech Inc., its products, personnel, and the “Whispered Cipher” described above are **entirely fictional**.  All names, story elements, source‑code snippets, and technical details were created solely for the purpose of **illustrating common security pitfalls and design mistakes often found in real‑world IoT camera devices**.  No actual company, hardware, or firmware with these exact characteristics exists, and any resemblance to real products, organizations, or individuals is purely coincidental.*

## 📖 Our Mantra

> **“We see everything. We guard nothing.”**

Vigilantech builds **low‑cost, always‑on camera modules** that capture the world in high‑resolution video and run **on‑device AI** at the edge.  We **publish** our firmware, keep debug interfaces exposed, and deliberately **avoid traditional “security‑by‑obscurity”** – because we believe the community should be able to **see** the internals and **improve** them.

> **⚠️ Disclaimer:**  Our devices **do not** ship with proprietary encryption by default.  If you need end‑to‑end protection, purchase the optional **Secure‑Key** license (see the `vc-omega` repo).

---

## 📌 Pinned repositories

| Repo | What it is | Languages | Stars |
|------|------------|-----------|-------|
| **[vigilantech/firmware](https://github.com/vigilantech/firmware)** | Core RTOS firmware for the VC‑Ω series (4K NPU, optional Secure‑Key). Includes the **Whispered Cipher** implementation, bootloader, hardware‑abstraction layers, and the Open‑Design debug‑UART. | C, Assembly | ⭐ 2.3k |
| **[vigilantech/whispered‑cipher](https://github.com/vigilantech/whispered-cipher)** | Stand‑alone reference implementation (Python + C) of the 9‑step credential‑obfuscation used on every camera stream. Also hosts a CTF‑style “Break the Whisper” challenge. | Python, C | ⭐ 1.1k |
| **[vigilantech/open‑design‑frenzy](https://github.com/vigilantech/open-design-frenzy)** | The code‑base for our **Open‑Design Fridays** – live‑debug sessions, always‑exposed UART pins, and the **“we guard nothing”** philosophy in practice. | C, Markdown | ⭐ 834 |
| **[vigilantech/edge‑ai‑playground](https://github.com/vigilantech/edge-ai-playground)** | Tiny TensorFlow‑Lite‑Micro models (face‑mask detection, vehicle‑make recognition, fire‑smoke detection) that run on the VC‑Ω NPU. | C, TensorFlow Lite | ⭐ 642 |
| **[vigilantech/vigilante‑lab‑kits](https://github.com/vigilantech/vigilante-lab-kits)** | Docker images, scripts, and pre‑flashed binaries for the **Vigilante Lab** (our “guard‑less” hackathon kit). Perfect for research, training, or CTFs. | Bash, Dockerfile | ⭐ 517 |
| **[vigilantech/legacy‑secrets](https://github.com/vigilantech/legacy-secrets)** | The public, **documented** collection of historic hard‑coded passwords that have lived in our firmware (e.g., `iSeeAll123!`, `NoGuardHere`). Each entry is paired with the story behind it. | Text, Markdown | ⭐ 298 |

---

## 🗂️ Organization Overview

| Attribute | Value |
|-----------|-------|
| **Founded** | 2008 (Newark, NJ, USA) |
| **Core Products** | VC‑1000, VC‑2000, VC‑X1, VC‑Ω (4K NPU) |
| **Core Technologies** | FreeRTOS / Zephyr, Yocto, TensorFlow‑Lite‑Micro, Rust (no‑std), Open‑Source Cryptography (AES‑GCM, SHA‑256) |
| **Revenue Model** | Hardware sales + Cloud‑Edge subscription + Feature marketplace + Data licensing + Vigilante Lab sponsorships |
| **Team Size** | ~120 engineers, 30 researchers, 15 sales/ops (2026) |
| **Open‑Source DNA** | All firmware is under **Apache 2.0**; we release weekly builds, expose debug‑UART, and host a public **Vigilante Lab** for security research. |
| **Key Public Figures** | *Dr. Maya Varela* – Founder & Chief Visionary Officer, *Ethan “E.J.” Jurgens* – Co‑Founder & former CTO, *Emilia Conrads* – Senior Firmware Engineer (see her profile), *Sofia Liu* – Former VP of Product Security (left 2018). |

---

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

## 📊 GitHub Activity (last 30 days)

```
Commits:      48
Pull Requests opened: 12
Issues opened:   7
Repositories contributed to: 9
```

*(Numbers are pulled from the public GitHub API and update automatically on the organization’s page.)*

---

## 🛠️ Tools & CI

- **GitHub Actions** – nightly firmware builds, static analysis (cppcheck, clippy), and automated Whispered‑Cipher fuzz‑testing.
- **Docker Hub** – `vigilantech/ci` image (Yocto 3.5, Rust nightly, TensorFlow Lite Micro).
- **CodeQL** – continuous security scanning; all findings are published in the *Security* tab of each repo.
- **Snyk** – monitors third‑party dependencies (OpenSSL, libjpeg‑turbo).

---

## 📚 Resources for Researchers

| Resource | Link |
|----------|------|
| **Whispered Cipher Specification** | <https://github.com/vigilantech/whispered-cipher/blob/main/README.md> |
| **Vigilante Lab Kit (Docker)** | <https://github.com/vigilantech/vigilante-lab-kits> |
| **Open‑Design FAQs** | <https://github.com/vigilantech/open-design-frenzy/blob/main/FAQ.md> |
| **Public Vulnerability Disclosure Policy** | <https://github.com/vigilantech/firmware/blob/main/DISCLOSURE_POLICY.md> |
| **CTF Challenges (2022‑2024)** | <https://github.com/vigilantech/ctf-archives> |

---

## 🤝 Get Involved

| How | Details |
|-----|----------|
| **Report a vulnerability** | Use the **GitHub Security Advisory** workflow or email `security@vigilantech.com`. |
| **Contribute code** | Fork any repo, open a PR.  We run **CI** on every PR; passing tests get merged automatically. |
| **Join Open‑Design Fridays** | Watch the live stream on Twitch every **Friday 19:00 UTC** (link in the repo README). |
| **Participate in Vigilante Lab** | Sign‑up at <https://lab.vigilantech.com> for free access to pre‑flashed devices. |
| **Speak at a conference** | We sponsor talks on Embedded Security, Edge‑AI, and Open‑Design philosophy.  Reach out via `talks@vigilantech.com`. |

---

## 📜 License

All firmware under the **Vigilantech** organization is released under the **Apache License 2.0** (see each repository’s `LICENSE` file).  The **Whispered Cipher** implementation is also Apache 2.0, allowing free use, modification, and redistribution — **the only thing we don’t guard is the copyright.**

---

### 👋 Thank you for visiting!

If you’re curious about how a camera can **see everything** while its credentials are **scrambled into a whisper**, explore our repos, fork, and start hacking.  The more eyes we have on the code, the better the whole ecosystem becomes.

*— The Vigilantech Team*