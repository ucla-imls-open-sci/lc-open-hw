---
title: "Lesson 3: licenses and open science hardware"
teaching: 20
exercises: 10
---

:::::::::::::::::::::::::::::::::::::: questions 

- What licensing options exist for open hardware?
- How can librarians help researchers choose a license?


::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Identify the most relevant open hardware licenses.
- Understand the differences between them
- Recommend a license based on a researcher’s goals.

::::::::::::::::::::::::::::::::::::::::::::::::

## What is an open source license?
Licensing is a critical part of making hardware “open.” For researchers working on open science hardware (OSH), selecting an appropriate open license—or understanding one that’s already in use—can determine whether a design is reusable, modifiable, and legally shareable. As librarians, you can help researchers make informed decisions about how to license their work or how to assess the reusability of existing designs.

Open source licenses are legal tools that define how others can use, modify, and distribute a project. In open science hardware, licenses perform two key functions: they guarantee user freedoms and set the conditions under which those freedoms are granted. These licenses originate in the free and open-source software (FOSS) movement and have since been adapted for hardware contexts.

Open licenses are not the same as placing something in the public domain. While public domain tools like Creative Commons Zero (CC0) waive all rights, open licenses retain copyright but grant specific permissions, usually with obligations—such as requiring attribution or ensuring derivatives remain open. This structure fosters collaboration while protecting the author’s intentions.


::: callout

The latest version of the CERN-OHL is one of the most widely used licenses for open hardware, providing a suite of strong copyleft, weak copyleft and permissive alternatives

:::

## Why licensing matters for OSH

Unlike software, open hardware projects combine multiple types of materials: physical designs, documentation, firmware, and often branding. This makes licensing more complex. It’s not uncommon to find a project labeled “open” that uses a valid open license for its documentation, but offers no instructions or files to actually reproduce the hardware. 

Licenses for OSH fall into two broad categories:

- Copyleft licenses (like CERN-OHL-S or TAPR OHL) require that any modifications or derived designs are also shared openly under the same terms. These are useful when a researcher wants to ensure that improvements remain part of the commons.

- Permissive licenses (like Solderpad or CERN-OHL-P) allow for reuse with minimal restrictions, including commercial use and incorporation into proprietary designs. These can help maximize adoption but don’t require that others contribute improvements back.

The CERN Open Hardware Licence (OHL) is currently one of the most widely recommended licenses in OSH. Its three variants—strongly reciprocal (CERN-OHL-S), weakly reciprocal (CERN-OHL-W), and permissive (CERN-OHL-P)—allow researchers to choose the level of openness and control they’re comfortable with.

![Permission overview for software licences, from The Turing Way](fig/lic.png)

When helping a researcher choose a license or evaluate an existing one, consider the following questions:

- Does the license clearly allow use, modification, and redistribution?
- Is the license compatible with the researcher’s goals—e.g., wide adoption, community building, or commercial integration?
- Does the project apply the license consistently to all parts of the work (hardware design files, software/firmware, documentation, branding)?
- Is attribution required, and are there clauses about how derivatives must be shared?

For projects aiming for certification, the [OSHWA Certification Program](https://certification.oshwa.org/) provides guidance on applying appropriate licenses to each component—hardware, software, documentation, and branding—and helps clarify the distinction between open and partially open projects.


::: challenge 

## Challenge 1: Copyleft or not?

A researcher asks if they should use a copyleft or permissive license for their new design they’re working on. Write two pros and two cons of each approach.

::: solution 

## Some possible answers

### Copyleft licenses
Pros:

-    Keeps all future versions open

-    Encourages community contribution

-     Protects against proprietary forks

-     Ensures openness long-term

Cons:

-     Can limit commercial adoption

-     May scare off potential collaborators

-     Legally more complex

-     Slower spread in industry

#### Non-copyleft
Pros:

-    Easy for anyone to adopt

-    Encourages wider use

-    Attracts industry partners

-    Simple legal terms

Cons:

-    Others can close off derivatives

-    No obligation to share improvements

-    Can lead to privatization of work

-    Community benefits less guaranteed

:::

## Common pitfalls and how to address them

Many OSH projects still use software licenses (like GPL or MIT) or Creative Commons licenses without fully understanding their implications for hardware. This can lead to confusion or legal uncertainty. For example, Creative Commons licenses aren’t designed for functional objects, and standard software licenses might not account for physical reproduction or patent rights.

We should encourage researchers to:

- Choose a hardware-specific license (e.g. CERN OHL or Solderpad).
- Be explicit about which license applies to which component of their project.
- Avoid mixing incompatible licenses.
- Document their licensing choices clearly in a README or metadata file.

Tools like [ChooseALicense.com](https://choosealicense.com/) now include hardware options and can help researchers navigate their choices with plain-language explanations.


::: callout

Licenses that include non-commercial (NC) or no-derivatives (ND) clauses—like CC BY-NC or CC BY-ND—are not considered open source because they limit how others can use, modify, or build upon your work. For hardware to be truly open, others need the freedom to reuse, adapt, and redistribute—including for commercial and derivative purposes.

Learn more about this here: [Why are Creative Commons 'Non Commercial' licenses not Open Source and a big problem for hardware & product design - Mifactori](https://mifactori.de/non-commercial-is-not-open-source/)

:::
::: challenge 

## Challenge 2: Licenses in real projects

Find an example of a project using CERN-OHL and summarize why this license fits the project.

::: solution 

# Possible answers
- Projects in the Open Hardware repository (https://ohwr.org/)
- Projects in the OSHWA list, filtered by CERN license (https://certification.oshwa.org/list.html)

:::


::: keypoints 

- Licensing grants others the legal rights to use, modify, and redistribute a design.
- OSH projects often involve multiple license layers—for hardware designs, documentation, software, and firmware.
- Two main types of open licenses: Copyleft (e.g. CERN-OHL-S, TAPR OHL), requiring that any derivatives are shared under the same license; Permissive (e.g. Solderpad, CERN-OHL-P), allowing broad reuse with minimal restrictions, including in proprietary contexts.
- The CERN Open Hardware Licence v2 is the most used one, and offers three variants (Strong, Weak, Permissive) to suit different openness levels.
- Not all Creative Commons licenses are truly open source—those with NC (Non-Commercial) or ND (No Derivatives) clauses restrict reuse and are not suitable for OSH.


:::
