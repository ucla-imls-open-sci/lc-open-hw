---
title: "Introduction: What is open science hardware?"
teaching: 20
exercises: 10
---

:::::::::::::::::::::::::::::::::::::: questions 

- What is open science hardware (OSH)?
- Why is OSH important in academia?
- What are examples of OSH projects?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Define open science hardware
- Describe how OSH benefits reproducibility, access, and innovation
- List at least 3 concrete examples of OSH in research or education.

::::::::::::::::::::::::::::::::::::::::::::::::

## Why a course for librarians?

Librarians already work with much of what makes open science hardware (OSH) useful: open data and open software, git forges and repositories, licensing, citation, and the local research community. Three things make librarians well placed to support OSH:

-   **Reach.** Each librarian supports many researchers, so one librarian who knows where to look and what to ask can help many projects.
-   **Findability.** Librarians know metadata, discovery and how to evaluate sources, and hardware designs are hard to find.
-   **Publication.** Librarians know how research outputs are deposited, described and cited, and designs need the same.

This course is different from one for scientists. You will not learn to build hardware. You will learn enough about it to help researchers who build, find, share and cite it.

## Warm-up: what do you already know?

Start by sharing what you work on, what you already know about OSH, and what you think it is. Then do the jargon buster below. OSH comes with a lot of vocabulary, and some of it is new to everyone.

::::::::::::::::: challenge

## Warm-up: jargon buster

In a shared document (Etherpad, Google Doc or whiteboard), add a short definition next to any term you know, and a "?" next to any term you don't. If someone else has added a "?" and you can answer it, answer it. Keep each entry to one line, and do not look anything up. You have 3 minutes.

::::::::::::::::: solution

## What to expect

Some terms will have several definitions and some will stay as "?". That is fine. The goal is a shared glossary that the group builds together and comes back to, not agreement on every term. The episodes explain each term when it comes up.

:::::::::::::::::
:::::::::::::::::

::: instructor

Keep this to about 8 minutes in total. It is a warm-up, not a lesson. Participants add what they know, and you do not define terms for them.

**Before the session.** Create a shared document that participants can edit without logging in, and paste in the term list below. Leave one empty line under each term.

**Term list to copy and paste:**

```
Open source:
Open science hardware (OSH):
FAIR:
Prototype:
Bill of materials (BOM):
Firmware:
Copyleft:
Fork / remix:
Calibration:
OSHWA:
```

Edit the list if your group differs. A mix of terms participants probably know (open source, FAIR) and probably do not (firmware, copyleft, BOM) works best.

**Running it.**

1.  Share the link and show a timer. Give 3 minutes to add definitions and "?" marks.
2.  Spend 3 to 4 minutes on the terms with the most "?" marks. Read each one out and ask: "Does anyone want to take this one?" Do not define terms yourself unless nobody can.
3.  Leave anything unresolved as "?". Say that each term gets explained in the episodes.
4.  Keep the document open. Point back to it when a term comes up, and ask the group to add to it during the course.

**Keeping it short.** Cap the skim at the timer, whatever is left. Do not go through every term, do not correct partial answers at length, and do not let one term turn into a discussion. If the group is enjoying it, offer to continue during a break.

**Optional follow-up.** At the end of the course, return to the document and ask what changed, and what the group would add or fix.

:::

## Background: complex challenges, open opportunities

The challenges we are facing in the 21st century call for a more democratic, collaborative, all hands on deck approach to science and technology. But to participate in research, people need tools. Ideally, tools that would allow anyone to locally pursue the research questions they are seeking to answer.

During the last decade, following the ideas of [free and open source software](https://en.wikipedia.org/wiki/Free_and_open-source_software) and seizing the opportunities opened by the [maker movement](https://en.wikipedia.org/wiki/Maker_culture), more and more people started building their own tools for research. Taking the “open” in open science one step further, they release their creations or modifications under open licenses, sharing them through different internet platforms so anyone can build, study, modify, or commercialize them.

This practice, or “open science hardware (OSH)”, is growing worldwide. 

::: callout

In their 2021 Open Science recommendation, UNESCO defines open science hardware as *"the design specifications of a physical object which are licensed in such a way that said object can be studied, modified, created and distributed by anyone, providing as many people as possible with the ability to construct, remix and share their knowledge of hardware design and function."*

:::

## What counts as "open"?

"Open" is used in several related ways, and they do not mean exactly the same thing. Three definitions come up most often in this course:

-   The **Open Source Definition** of the Open Source Initiative (OSI), written for software.
-   The **Open Source Hardware Definition** of the Open Source Hardware Association (OSHWA), written for physical designs.
-   **Open science hardware**, as described in the UNESCO definition above, which adds the aim of making hardware for research available to as many people as possible.

![Venn diagram of three overlapping circles: the OSI open source definition, the OSHWA open source hardware definition, and UNESCO open science hardware. The overlap in the centre reads "Anyone can study, modify, make and share".](fig/open-definitions-venn.svg)

What they share is the idea that other people should be able to study, modify, make and share the work. They differ in what they cover (software or physical things), who they are written for, and how much they say about research. The diagram is a simplification, and real projects often sit between definitions.

::::::::::::::::: challenge

## Grey areas: does it count as open hardware?

Discuss each case with a neighbour. Is it open hardware? What would you need to know to decide?

1.  A natural history museum shares high-resolution 3D scans of shells so that researchers can print copies.
2.  A lab publishes the code for a sensor, but the circuit design files are only available "on request".
3.  A project shares its design files, but under a license that forbids commercial use.
4.  RISC-V is an open specification for computer chips, developed at UC Berkeley. Anyone can build chips from it.

::::::::::::::::: solution

## Some things to consider

1.  The scans are a digital file, and the printed shells are copies of a natural object, not a designed device. Whether it is "hardware" depends on what you mean by the word, and the licence on the scans matters. It is a good example of the edge of the definition.
2.  Open software on closed hardware is not open hardware. Files available only on request are a barrier to the freedom to study, modify, make and share.
3.  Licenses with non-commercial clauses are not considered open source (see Lesson 3), so this project would not meet the OSHWA definition.
4.  RISC-V is a specification, not a physical device, so it does not match the UNESCO definition of a physical object. It is open hardware in the chip design sense, and shows how much the word covers.

There is not always one right answer. The point is to see which questions to ask.

:::::::::::::::::
:::::::::::::::::

## Why are researchers using and developing OSH?

Today, researchers in academia have a hard time making science hardware work for their own needs. Science tools can be considered what we call black boxes: we know what goes in and what we get back, but we have limited or no information on their internal workings or design. This is a significant problem for science in terms of reproducibility, but it also has other consequences.

For scientists, black boxes are a problem because they make it difficult to source, maintain and adapt tools to different needs. Science often demands adapting experimental settings to new research questions; collaborative research with communities or citizen science projects often presents needs that were not originally conceived in the design of science hardware. The lack of access to blueprints combined with the niche, highly-specialized nature of science increases labs' dependence on centralized vendors; only some can afford the extra costs and delays.

Beyond customization, most of the tools used in research today are unevenly distributed. Science infrastructure is usually available to highly skilled experts, well-funded laboratories, and renowned institutions in countries with high investments in science and technology. For many scientists with limited budgets, access to the tools for research is hampered by prohibitive import taxes, lack of access to technical support, or inability to source spare parts. It becomes even more difficult for those communities aiming to participate in research in non-conventional settings, outside academia.

![Domains of open science, including open hardware, from the 2021 UNESCO Open Science Recommendation](fig/unesco.png)

::: instructor

This section is good for learners to exchange their own experience with science

:::

## Advantages of open science hardware

In this context, developing and using OSH gives researchers much better control over their experiments, and access to research that wouldn’t be possible with conventional proprietary instrumentation.

There are several benefits of OSH, including:

1. **Research integrity:** Research is inherently iterative, where we always build on past knowledge. Making hardware designs open source for others to study, peer review, reuse, and improve demonstrates accountability and commitment to the scientific process.

2. **Replicability:** Open Source Hardware designs can be replicated, allowing for verification and reproduction of experiments and data. Moreover, users can have much better control on the calibration of their devices, boosting replicability even further.

3. **Innovation:** By making OSH designs open source, others can collaborate on the design process leading to faster development, better products, and a larger user base for OSH instruments. Everyone benefits, as new designs do not need to start from scratch and designers of original instruments get access to derivatives of their work without having to develop things themselves.

4. **Accessibility:** OSH can make research more accessible, inclusive and diverse as the availability of designs allow anyone, anywhere to replicate and use hardware to test emerging ideas, and collect data, independently from who and/or where they are.

5. **Flexibility:** OSH allows researchers to quickly put together designs to test new research questions in an accessible way. With less risk, researchers can explore a new direction before committing more resources or using shared facilities that imply greater bureaucracy. Using rapid prototyping tools and open source licences scientists can adapt their experiments to their needs, and share these changes so others can do the same.

6. **Parallelisation:** Because the designs are open, a lab can build or source several copies of a device instead of depending on a single vendor unit. Where that is practical, running copies in parallel can speed up data collection and make it possible to collect types of data that would be too cumbersome to gather one run at a time. Cost varies a lot between projects (parts, build time and maintenance all count), so OSH is not automatically cheaper than a commercial device.

7. **Sustainability:** OSH designs can be more sustainable than proprietary products because they can be repaired and modified, extending the lifespan of the product and reducing waste. And in the case of the supplier going out of business, users and/or third party companies can keep systems running. 

8. **Education:** OSH designs can be a valuable educational tool, allowing students and researchers to learn from it, and fully understand how a certain tool is capable of capturing data on specific phenomena/events. This in turn opens up the opportunity for the design of better experiments and better control of data being output by equipment. 

::::::::::::::::::::::::::::::::::::: callout

How does OSH align with FAIR principles?

People in the community are working towards alignment with FAIR, to make OSH:
- Findable: Projects are shared with searchable metadata on open platforms.
- Accessible: Designs are available online under open licenses—no paywalls or restrictions.
- Interoperable: Uses standard, widely accepted formats like STL or CSV, and modular designs that work well with other systems.
- Reusable: Complete documentation and clear licensing make it easy for others to build, adapt, and improve on the work.

::::::::

:::::::::::::::: challenge 

## Challenge 1: OSH and libraries

Identify three ways in which open science hardware aligns with library values of access and preservation.

:::::::::::::::: solution 

## Possible answers
 
**ACCESS**
- It makes science tools available to more people: Just like libraries help people access books and info for free, OSH makes lab equipment and tools available without needing to buy expensive commercial stuff.

- Helps level the playing field: A small university or school with limited funds can build tools using OSH designs, giving more people a chance to do real science.

- Encourages learning by doing: Since people can build and modify the hardware, it’s like having hands-on learning resources, which libraries often promote.

- Supports community-driven knowledge: OSH is often built and improved by communities, similar to how libraries value sharing knowledge openly.

**PRESERVATION**
- It documents everything: OSH projects usually include manuals, design files, parts lists, etc. That makes them easy to reproduce and store—just like libraries archive useful information.

- It keeps knowledge from disappearing: If a company stops making a tool, you’re stuck. But if it’s open, the design still exists and can be reused or repaired later.

- Formats and licenses make reuse easier :Like how libraries like open formats (PDF, CSV, etc.), OSH encourages using accessible formats and clear licenses, so designs can be preserved and reused easily.

- People can adapt and remix the designs: like preserving not just the object, but the idea behind it—so others can build new things from the old.

- It’s sustainable: by enabling repairs and upgrades instead of throwing things away, OSH supports long-term use and reduces waste—something libraries increasingly care about.

:::::::::::::::::::::::::::::::::
:::::::::::::

## Examples of OSH in academia and beyond

### Neuroscience: [Open Ephys](https://open-ephys.org/)

Open Ephys is an open-source, employee-owned cooperative that aims to make neuroscience research more accessible by providing high-quality, affordable tools for electrophysiology. Founded in 2014, it supports researchers in building their own open-source rigs and promotes community ownership of scientific tools. By focusing on collaboration, open standards, and alternatives to commercial systems, Open Ephys helps reduce duplication of effort and fosters innovation across the global neuroscience community.

![Open Ephys piece of equipment](fig/oe.jpg)

## Conservation ecology: Audiomoth - [Open Acoustic Devices](https://www.openacousticdevices.info/)

AudioMoth is a low-cost, open-source audio recorder designed for environmental and biodiversity research, capable of capturing both audible and ultrasonic sounds. Originally funded by UK research councils, it has been widely used to monitor wildlife and detect illegal activities impacting ecosystems, such as tracking jaguar and puma populations. Its affordability and open design have led to broader applications, including studies on human health and noise pollution. Now developed and distributed by Open Acoustic Devices, AudioMoth can be bought pre-assembled or built using freely available design files.

![An Audiomoth in the wild](fig/audiomoth.png)

## Microscopy: [OpenFlexure](https://openflexure.org)

OpenFlexure is a high-precision, 3D-printed microscope designed to be affordable, customizable, and easy to maintain, making it ideal for education, research, and even healthcare applications. Originally developed at the University of Bath and now co-developed with STICLab in Tanzania, it combines traditional microscope objectives or a Raspberry Pi camera with submicron stage precision. Its open, modular design allows users around the world to adapt the tool for needs like water quality testing or malaria diagnosis. By relying on locally printable parts, OpenFlexure enables communities to build and repair their own scientific equipment without costly servicing.

![Latest version of the OpenFlexure microscope](fig/openflexure.jpg){alt='Latest version of the OpenFlexure microscope'}

::::::::::::::::::::::::::::::::::::: challenge 

## Challenge 2: Find open science hardware projects

Use a simple browser search and list the three most interesting open science hardware projects you can find online.

::::::::::::::::::::::::::::::: solution 

Many possible answers!

:::::::::::::::::::::::::::
::::::::::::::::::::::::::


::::::::::::::::::::::: keypoints 

- Open science hardware (OSH) makes scientific tools freely available to study, build, and adapt—supporting transparency and innovation.
- OSH addresses the limitations of proprietary “black box” tools by promoting reproducibility, accessibility, and customization.
- It empowers researchers worldwide, especially those with limited resources, to participate in and contribute to science.
- Examples of open science hardware can be found in most academic fields, with salient examples in neuroscience, environmental monitoring and microscopy 

::::::::::::::::::::::::
