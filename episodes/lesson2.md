---
title: "Lesson 2: How does open science hardware work?"
teaching: 20
exercises: 10
---

:::::::::::::::::::::::::::::::::::::: questions 

- Who is making open science hardware and for whom?
- What is shared in open science hardware?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Be aware of the diversity of open science hardware projects and how it impacts documentation
- Understand the main elements of open science hardware projects

::::::::::::::::::::::::::::::::::::::::::::::::

## Multiple ways of producing open science hardware

Open science hardware is created through a variety of pathways, reflecting the wide range of people and institutions engaged in science. As a result, documentation can be found in multiple, and often non-academic, publication venues. 

Some designs emerge from DIY or maker communities, where individuals use accessible digital fabrication tools—such as 3D printers or microcontrollers—to develop low-cost, adaptable solutions. Other hardware originates in academic and research institutions, often in response to specific scientific needs. In these cases, researchers may document and share their work through scholarly publications or institutional repositories. 

There are also collaborative efforts, such as hackathons or international gatherings like GOSH (Gathering for Open Science Hardware), where interdisciplinary teams co-develop tools with input from scientists, engineers, educators, and community members. These communities often run their own forums, where documentation can be found either in repositories or websites/wikis.

Finally, some commercial initiatives have adopted open hardware principles, releasing product designs under open licenses to foster community engagement and innovation. In these cases, a company website is probably the best source of information on that specific open hardware design.

::: challenge 

## Challenge 1: Meeting people where they are

Imagine a researcher at your institution has developed a custom sensor and wants to make it openly available. Based on what you’ve learned about the diversity of OSH practices, list two questions you would ask to better assess their choice.

::: solution 

## Some possible answers
- Where do you plan to share the documentation?
- Who is the intended audience or user community for your sensor?
- What kind of documentation have you prepared?
- Are you collaborating with any community or platform that supports open science hardware?
- Have you chosen a license that allows others to freely reuse and adapt your design?
- Are you considering publishing your work in a formal or informal venue?
- Are you aiming to make the sensor easy to reproduce using accessible tools?
- Would users need specialized equipment or knowledge to build or use the sensor?

:::

## From idea to prototypes and more

Open science hardware projects, like other research tools, typically begin with a clear problem or need identified by the researcher or developer. This need is gradually translated into desired features—the specific functions or capabilities the hardware should offer. 

With access to affordable rapid prototyping tools such as Arduino boards, laser cutters, or 3D printers, researchers can now create and test multiple hardware concepts quickly. These early iterations are used to explore technical possibilities and gather feedback from potential users.

For librarians supporting researchers, it’s helpful to recognize that open hardware development is often iterative. A researcher may begin with a simple prototype—something functional but rough—that allows them to experiment with certain features. Through multiple cycles of testing and improvement, a more stable version may emerge. 

At this stage, the design may be called a demonstrator: it works and meets the intended need, but may still require manual adjustments, lacks full documentation, or depends on custom parts. Only after thorough refinement, testing, and documentation does the hardware reach the stage of a product—something that others can reliably build or even manufacture.


::: callout

While most OSH documentation begins once the design reaches the demonstrator stage, open science advocates encourage sharing from the very beginning—even during the problem-definition phase. 

:::

Documenting decisions, trade-offs, and failed experiments can benefit others in the community and foster a culture of transparency and learning. As librarians, encouraging researchers to share early—and helping them organize and preserve that documentation—can play a key role in making hardware development more collaborative, discoverable, and reproducible.

## What is shared in open science hardware?

In the context of open science, sharing hardware goes beyond publishing a paper or uploading a schematic. Librarians can play a key role in guiding researchers toward comprehensive documentation practices, ensuring that shared hardware is both reproducible and impactful.

For a design to be truly open and reusable, it must include a comprehensive set of materials. The core “source” in open hardware typically consists of what we call design files that describe how the hardware is built. 

Depending on the nature of the hardware, the design files can include circuit diagrams, CAD models, layout plans, files for 3D-printing or more. If the project includes programmable elements, source code or firmware should also be shared. 

Open hardware should include a detailed bill of materials (BOM), outlining every component needed, along with technical specifications and sources. Assembly instructions, often with visual aids or videos, guide users through construction and setup. Well-documented projects often include information on testing and calibration, helping users assess the tool’s performance. 

All these elements should be accompanied by clear and open licensing, ensuring that others can legally reuse, adapt, and redistribute the work. 

::: callout

A README file is a plain-text document that gives an overview of a project and guides users on how to use, build, or contribute to it. In open hardware, it typically includes the project’s purpose, key components, setup instructions, links to design files, and licensing information. It’s often the first thing someone reads—so clarity and completeness are essential.

:::

## Barriers in open hardware

While efforts to standardize how open science hardware is documented, discovered, and evaluated have grown over the past decade, significant challenges remain—many of which are directly relevant to librarians supporting researchers. 

Since the OSH definition was first introduced, various initiatives have worked to align practices around openness. In reality, however, implementations across projects and organizations still vary widely. 

One of the core challenges lies in differing interpretations of what “open” means in practice. It’s not unusual to encounter projects that are technically open-licensed but lack the necessary design files, build instructions, or supporting information to enable real reuse. 

For librarians, this poses a key concern: a license alone does not guarantee accessibility or usability. Without proper documentation, researchers may struggle to replicate or build upon existing work, limiting the collaborative and inclusive potential of open hardware.

::: challenge 

## Challenge 2: Reusing existing designs

You’re working with a researcher who wants to reuse an open hardware design for a lab tool. They’ve found a promising project online. What questions would you ask to identify if the project is usable?

::: solution 

# Possible answers
- Is the documentation complete and clear?
- Is the license open and does it allow reuse and modification?
- Has the hardware been tested or used by others?
- Are the materials and components easy to source?
- Is there community support or a place to ask questions?
- Is the design up to date?
- Is it adaptable to your lab’s specific needs or constraints?
– Was it developed in a reliable context (e.g., research lab, maker community, company)?

:::


::: keypoints 

- OSH is developed by a wide range of actors—from academic labs and companies to DIY communities and grassroots collaborations.
- Good documentation includes: design files, bill of materials (BOM), source code or firmware (if applicable), assembly instructions, testing/calibration data, and a clear open license.
- Librarians can support researchers by helping assess documentation completeness and encouraging early sharing—even before a design is finalized.
- Not all “open” projects are truly reusable—many lack the documentation needed for others to replicate or adapt them.


:::
