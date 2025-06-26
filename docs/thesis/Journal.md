---
hide:
  - navigation
  - toc
  - title
---

# Explorations and Journal
<div style="height:2px; background-color: #E17858; margin-top: 40px; margin-bottom: -20px;"></div>

- I asked ChatGPT to make a small summary of each month's refections (I talk a lot so this is better). If you want to understand all my process than this is it, if you are more interested in the interventions and the analysis than see the next the *Interventions SIte* and if you want to see the part of the deliverable than go to *Final Deliverable*

## Term1: Mapping the Terrain and Defining Intentions
**October:**
In October, the focus was on understanding the current landscape of AI and defining the intentions for the thesis. Through conversations with professionals and the TANIA chatbot project, I began exploring how AI could be used not just for creativity, but also for community support and fabrication. These early explorations helped me realize AI’s potential as an accessible tool for knowledge and empowerment.

This month was mainly about mapping possibilities: identifying what tools exist, what’s missing, and where AI might fit into design and fabrication spaces. It was also a moment to reflect on whether this work should be aimed at businesses or communities, and whether it could support real fabrication rather than just aesthetics. No prototypes were built yet; this was about setting the direction.

**November**
In November, I focused on exploring AI both as a creative companion and as a practical tool for fabrication. I experimented with platforms like Vizcom, Meshy, LumaLabs, and Krea to understand how they support 3D modeling and design. While these tools proved helpful for generating and rendering concepts—like designing a chair and viewing it from multiple angles—I also realized their limitations when it comes to actual fabrication. The outputs often lacked the precision or structure needed for real-world making.

At the same time, I prototyped an AI assistant bot through a GitHub repository that worked via Telegram, allowing users to share messages, photos, or audio to get fabrication help. While the bot technically functioned, it lacked a clear use case and required a paid API, which made accessibility and context a problem. This month highlighted the need to move beyond general-purpose tools and begin thinking about what kind of AI interactions are truly useful and intuitive in makerspace environments.

**December**
In December, the thesis moved from theoretical exploration into hands-on experimentation. The goal was clear: test if AI could be used to fabricate real objects through natural language inputs, with minimal human involvement. Projects like “make me an organic lamp” served as test cases to explore AI’s potential to generate printable objects from simple, subjective prompts.

What emerged was a split reality. AI could generate interesting shapes for simple items like chairs or vases — but it struggled with subjective language (e.g., “fun” or “organic”) and completely broke down when tasked with functionally demanding objects like lamps, which require structural reasoning, material constraints, or mechanical integration. While rendering and ideation tools offered exciting visuals, actual fabrication still required the user’s judgment and skill.

These limitations sparked a deeper shift in the project’s direction. It became clear that the real value of the thesis was not in making one specific object, but in developing a methodology — one that explores how AI could one day enable meaningful design and fabrication for everyone. If AI evolves to better understand physical constraints and function, what would that mean for everyday users and communities? Could people repair broken objects more easily? Design and fabricate solutions themselves? Could AI become an enabler of local, democratic making?

This realization led to new questions:

- Should the focus now shift toward community implementation?

- Do people need to be taught how to fabricate before AI can help them design?

- What would a useful AI interface or workflow actually look like in a makerspace?

In essence, December marked a turning point: from trying to make things with AI, to designing a framework for how AI could support future community-based making. The research shifted from “What can I make with AI now?” to “What kind of making could AI enable tomorrow — and how do we prepare for that today?”

## Term2: Mapping the Terrain and Defining Intentions
**January:**
In January, the project transitioned into a more grounded, application-focused phase. The emphasis shifted toward mapping community makerspaces and identifying potential contexts for AI integration. Three communities were selected as case studies, each representing different needs and possibilities:

- Ateneu de Fabricació de Gràcia – focused on accessible 3D modeling and improving the fabrication process.

- Lichen – a social innovation hub with potential for AI-driven community knowledge assistants.

- Biomaterial Altars – exploring AI’s role in supporting sustainable fabrication workflows.

The broader objective was to explore how AI could support three key pillars:

- Modeling Tools – using text, voice, or image inputs to generate 3D models.

- Fabrication Support – tools for error detection, troubleshooting, and print diagnostics.

- Design Assistants – AI systems that guide users through sustainability, materials, or design decisions.

This month also marked the first contact with a real makerspace, Ateneu de Gràcia. That interaction revealed a gap between available AI tools and community awareness. While staff were curious, their actual challenges didn’t align with receiving “pre-made” tools — they needed relevant support tailored to their workflow. This led to a shift in strategy: instead of pushing tools into the space, we proposed hosting an AI introduction conference to let the community define the needs AI might solve.

Simultaneously, I began developing custom tools:

- MegaTool (early version): a basic web platform where users could input text, image, audio, or webcam data to generate 3D models and receive basic 3D printability feedback.

- Rhino Files: a voice-based modeling tool that translated a user’s spoken narrative into a prompt suitable for a text-to-3D mesh model generator, demonstrating a hybrid natural language processing pipeline.

- ChatGPT for Print Troubleshooting: experiments with using ChatGPT to diagnose 3D print errors from images or files, which worked in a general sense but lacked deep contextual accuracy.

The biggest takeaway from January was that AI tools often need translation layers — systems or interfaces that make vague or subjective inputs (like user stories) into precise, actionable prompts. It also became clear that implementing AI in community spaces isn’t just about building tools, but understanding people’s workflows, expectations, and comfort levels.

This month pushed the project from concept to early prototypes and revealed the importance of co-designing with communities rather than designing for them.

**February**
February was a really important turning point in my thesis. It was the first time I had full, real contact with the communities of practice I wanted to work with. I ended up deciding to focus only on Fab Casa del Mig and Ateneu de Fabricació de Gràcia, and let go of Lichen and Biomaterial Altars. They’re still valuable communities to me personally, but I realized I was spreading myself too thin and needed to go deeper with fewer partners.

These two makerspaces are very different, which helped me see the range of needs and possibilities for AI. Fab Casa del Mig is super neighborhood-based, with the same people coming back again and again. It’s informal, friendly, and focused on learning and experimenting as a community. Ateneu de Gràcia is more structured and institutional — people come for specific projects and there’s a strong focus on giving back, like teaching others after using the space.

What really changed this month was that instead of me deciding what AI should do, they started telling me what would actually be useful. At Ateneu, it became clear that their biggest interest was in teaching the teachers — because they host different groups and don’t always have repeat users, it doesn’t make sense to push a complex tool onto people who are just passing through. They liked the idea of doing workshops and conferences to raise awareness and help educators understand how to talk about AI. They also brought up real, practical pain points — like how complex it is to go from image to vector to laser cut file — and asked if AI could help with that. But they were very cautious about keeping things human and hands-on, and not turning the space into a screen-based, isolated experience.

Fab Casa del Mig, on the other hand, was really excited about physical installations and prototypes — like a table with a camera that gives feedback on your 3D print, or voice interfaces that guide you through making. They wanted things that would be visible, interactive, and fun, and they were really interested in me teaching the community directly so they could explore AI together. They were much more open to using AI in playful and experimental ways, as long as it stayed rooted in the physical space.

While all of this was happening, I kept building and testing tools. I kept working on MegaTool, trying to improve how it handled inputs and outputs. I kept exploring mesh generation tools as new ones kept coming out. I also tried making objects like a jewelry holder using Vizcom, but ran into issues because tools like that are very visual and don’t really “understand” functionality — they didn’t recognize that holes needed to exist or had a purpose. I also tried designing an ergonomic chair, and while it looked cool, it was impossible to translate into something actually makeable.

The big realization this month was that AI doesn’t really understand function yet — it’s great at generating visuals, but not at making something usable or structurally sound. So instead of trying to make a universal AI tool that works for everyone, I started thinking more about methodologies: how do we introduce AI into these spaces in a way that supports the people who are already there, with their specific rhythms, needs, and values?

This month helped me stop thinking about AI as a solution to give people, and start thinking about it as a process to explore with them.


**March**
March was my first time teaching AI to others, and it raised a lot of ethical questions. I didn’t want people using tools they didn’t understand, so instead of a hands-on workshop, I ran conference-style sessions. At Ateneu de Gràcia, I taught AI to teachers — they were fascinated but also worried about what this means for the future of design. We agreed the next step was a proper workshop for the community. At Fab Casa del Mig, it was more playful — people explored tools like Krea but didn’t go very deep.

It was also the first time I tested MegaTool, and it didn’t go as expected. Just as I brought it to the community, the API I was using went private — and I realized that relying on external tools makes open-source projects fragile. Even if the code is open, the tools behind it aren’t. That made me question whether building AI-based prototypes for makerspaces makes sense at all — they’re hard to maintain, they break fast, and someone would always need to update them after I leave.

That’s when I started shifting from tool-making to methodology. AI in fabrication might not be about making a single device or app — it’s about helping communities understand the tools, ask the right questions, and use AI critically and creatively. My role became less about building something lasting, and more about starting a conversation that can last on its own.

**April**
April was strange but revealing. I gave a conference-style workshop to a private company and realized how different the expectations are compared to makerspaces. The same AI-for-design presentation that fascinated educators felt almost useless to professional designers. For them, modeling tools didn’t add much — they wanted AI to do the tedious work, like floorplans or adapting mechanisms, not help with creativity. That moment made it clear: AI is still in the research phase, and its value really depends on context.

This was also the month I officially let go of MegaTool. The API I was using went private just as I tried to open it to the community — and that made me reflect on how fragile open-source projects are when they rely on third-party tools. Even if the idea is good, maintaining something like this alone, for a community space, isn’t sustainable. I realized it’s not about building tools — it’s about building methods for how to use and question them.

At the same time, GPT-4’s new image capabilities opened new doors. I started experimenting with using AI for laser cutting, testing how it could help generate outlines and signs. It still couldn’t handle function (like making a box or generating the correct number of game pieces), but for things like converting text to simple outlines, it improved. I learned that text prompts worked better than image-based ones, especially when the goal was vectorizing something cleanly in Inkscape. Still, there were limitations: broken paths, no true object permanence, and a lack of design intent.

I also met with Pietro and Chris — developers working at the intersection of design and AI — and we all agreed: AI works better with code. Tools like Blender and OpenSCAD are more reliable because AI handles structured input better than messy meshes or prompts. That conversation helped shift my perspective again: maybe the best way to bring AI into makerspaces is not to teach people how to prompt, but to use AI to teach fabrication — through instructional bots, checklists, and support systems that guide people through processes like 3D printing or laser cutting.

So the focus turned toward knowledge-sharing and community literacy, not tool deployment. Because if AI can’t yet help people make things directly, it can at least help them learn how to make.


**May**
In May, I finally ran the full workshop, testing it across MDEF and Fab Casa del Mig, and preparing for Ateneu. The MDEF group — speculative designers — responded really well. They saw how AI could democratize design in makerspaces by giving more people access to tools and processes. But they also saw the difference between AI for community use and AI for business. In commercial settings, there's more pressure, responsibility, and ethical complexity — it's not just about learning or experimenting, it’s about production, profit, and consequences.

At Fab Casa del Mig, the group was more diverse — some took 30 minutes to log in, while others were experienced designers. The activities were playful and competitive, and while people enjoyed themselves, I noticed something recurring: designers want AI to do the tedious work, like floorplans and tech prep, not to help them imagine. And non-experts don’t always know how to question the tool, which makes it hard for them to use it meaningfully.

This made me rethink a lot. I realized the tools I’m developing for AI-based fabrication are too early-stage to be useful for designers, and too complex or unstructured for non-experts. MegaTool was a great idea in theory, but the open-source dream falls apart when the APIs behind it go private — and maintaining it in a community space long-term just isn’t realistic.

Most people still see AI as a “magic tool” that should automate effort, not amplify the process. But that’s not my view. I believe AI should support reflection and learning — not just speed things up. Unfortunately, everyone wants acceleration, not amplification. That’s the real tension.

AI for fabrication still lacks the maturity to deliver usable results, and if it develops into something hyper-efficient, we risk losing the learning process. Only people with a background in design will know how to challenge AI critically. That’s why I’ve shifted focus toward teaching people what AI is, how it works, and what to expect from it — not just how to prompt, but how to understand its limits.

If AI is to help in makerspaces, it may not be through software — maybe it’s a physical assistant, like a small robot or embedded system, that can explain how to use machines and free up human facilitators. But whatever it becomes, we need to keep asking: what is AI really for — and who is it serving? Because we’re not just using tools; we’re shaping how people learn, make, and imagine the future.

**June**
June was supposed to be the closing of my thesis — the end of the workshops and the beginning of some kind of conclusion. But honestly, it didn’t feel like a closing at all. I ran the final workshops at Ateneu de Gràcia and MDEFest, and while they echoed much of the feedback I’d already received — curiosity, ethical tension, excitement, and skepticism — what became clearest was that this project isn’t finished. It’s a mapping. A beginning. A big question with no single answer.

Throughout this journey, I tried to cover three enormous fields at once: AI in design, AI in fabrication, and AI in makerspaces. Each of these could have been a thesis on its own, and I now understand that in six months, the most valuable thing I could do was map the terrain — not solve it. AI is evolving fast. New tools are emerging that already do things I was struggling with just a few months ago — like breaking models into pieces or recognizing and modifying a design. It makes any attempt at a “final prototype” feel outdated the moment it’s built.

My original idea — the MegaTool — couldn’t survive the shift to private APIs, the speed of AI updates, or the real needs of communities. It taught me that building AI tools for fabrication isn’t just about tech — it’s about maintenance, relevance, and trust. And I’m not a programmer. I’m one person trying to navigate something that changes every two months.

The roundtable at MDEFest, where I presented the manifesto I’d been shaping since February, felt like a reflection of all my internal contradictions. I tried to collectively edit it with four professionals — a speculative designer, a product designer, a programmer, and a teacher — but the diversity of backgrounds made it almost impossible to reach consensus. Everyone agreed that AI is useful for creativity, not yet for fabrication, and that true democratization requires more than tools — it requires knowledge, time, and acess to tools.

They also challenged one of my core beliefs: that people shouldn’t use AI unless they understand how it works. They said it’s unrealistic — people use microwaves without knowing how they function. And while I still believe understanding AI is important, I see now how complicated that stance is, especially in community contexts.

So, what’s left? A workshop model, a set of ethical reflections, and a methodology — not a product. A community that now knows more about AI than it did before. And a lot of unanswered questions. Should I build a chatbot assistant for makerspaces? Should I create fabrication tools that speed up modeling? Should I focus on a single community and go deep? Or try to design a flexible solution for different spaces?

Right now, I don’t know. AI is still in a research phase, still unpredictable, still full of hype and magic-thinking. And I refuse to treat it like a miracle button. If we don’t teach people how to think critically about it — how to question, prompt, reflect, and understand its limitations — we’ll lose the point entirely. AI should amplify thinking, not replace it.

That’s the heart of my thesis. It’s not a final answer — it’s a call to stay curious, critical, and careful. And it’s a reminder that if we want AI to serve communities, we need to start by serving those communities ourselves — not with shortcuts, but with care.

