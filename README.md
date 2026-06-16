# Master Any College Course with Claude Project: Your Personal AI Tutor Playbook

## 📋 What You'll Learn

After completing this tutorial, you'll know how to build a Claude Project from scratch for any college course — integrating all your course materials into one place, creating a personalized AI tutor that understands your textbook, your assignments, and your learning progress, and establishing a sustainable system that gets better the more you use it.

## 🎯 Why Does This Matter?

Picture this scenario: You're taking Linear Algebra, it's 2 AM, you're stuck on a problem, your professor isn't available, and all your classmates are asleep. You're staring at the textbook, completely lost on what to do next.

Now imagine a different scenario: Same time, same problem, but you open a Claude Project specifically built for this course. This AI has already read your entire textbook, knows exactly what your assignment requires, remembers the concept you were confused about last time, and can adjust its explanations based on your level of understanding. All you need to say is: "Where did I go wrong on this problem?"

The second scenario isn't fantasy. This tutorial teaches you exactly how to build it.

More importantly, this method doesn't just work for Linear Algebra. Formula derivations in STEM courses, coding assignments in Computer Science, case readings in Law, financial analysis, close reading in Literature — for any college course, the underlying logic is exactly the same. Once you learn this approach, you've learned a study method that works for any subject.

---

## 📖 The Complete Method: Three Phases, One Setup, Lasting Benefits

### Phase 1: "Feed" the Textbook to AI

The first challenge — one that many people never think about — is the textbook's file size. A typical college textbook runs 700-800 pages, and uploading it directly to the Knowledge Base will exceed the file size limit. So before uploading, you need to "slice it up."

Take *Linear Algebra and Its Applications, 5th Edition* as an example — you can download it from [this link](https://broman.dev/download/Linear%20Algebra%20and%20its%20Applications%205th%20Edition.pdf). It's nearly 600 pages, too large to upload whole, but if you split it by chapter, each section is around 60-100 pages, well within the upload limit.

**Splitting a textbook** can be done with different tools depending on your preference. If you're on Mac, the built-in **Preview** app works great: open the PDF, go to View menu and switch to Thumbnails view, you'll see all page thumbnails on the left. Hold Shift and click to select the pages you want to extract, then drag them out or use File → Export as PDF to save those pages as a separate file. If you prefer online tools, ilovepdf.com has a dedicated "Split PDF" function — just specify page ranges. You can even ask Claude to write an automation script for you — that's itself a practice opportunity for using AI.

After splitting, if individual files are still too large, do one more step: **compress** them. Both ilovepdf.com and smallpdf.com have compression features that can typically reduce file size by 70-90% while keeping text content intact.

Upload all your split and compressed files by clicking the **"+"** button in the Files area on the right side of your Claude Project. Once uploaded, Claude can read and reference this textbook content in all conversations within this Project.

---

### Phase 2: Build the Complete Course Context

The textbook is just one of your course materials. A real course has many other resources: lecture notes from your professor, reference websites, assignment descriptions, past exam problems. This phase integrates all of these and helps AI use them effectively.

First, **organize your file names**. Before uploading, spend a few minutes giving all your materials clear, descriptive English names, like `lecture-01-intro.pdf`, `hw-1-description.pdf`, `reference-eigenvalues.pdf`. This step seems minor, but clear file names are essential for AI to find the right materials later. Upload all organized files to the same Project's Files area along with your textbook files.

After uploading, do the second thing: **create a materials index**. Open a new conversation, list all your file names and send them to Claude, asking it to generate a short index document — each filename followed by 2-3 sentences describing what the file is and what it contains. Have Claude generate this index as an Artifact, then click **"Add to Project"** in the top right corner of the Artifact to save it to the Knowledge Base.

The purpose of this index file becomes clear when you write your Instructions — you can tell AI "there's an index here; when you need a specific material, check the index first, then read the corresponding file." This way AI can retrieve materials on demand rather than trying to read everything at once.

Third, and most crucial for this phase: **write your Instructions and requirements document**.

**Instructions** are the system prompt you write in the Instructions area on the right side of your Project. They define this AI's role and behavior within this Project. You can send your requirements to Claude and have it draft one for you, then modify it based on your situation. Good Instructions should convey these ideas: this AI is a learning tutor for this course, its goal is to help you truly understand and internalize concepts, not just give you answers; it should gauge your understanding level from how you phrase your questions and adjust the depth of its explanations accordingly; it knows what materials are in the Knowledge Base (via the index); and at the start of each conversation, it should first read `progress.md` to understand your learning progress. We'll explain this last part in detail in Phase 3.

**Requirements document** is another important file, specifically for storing current assignment information. It's not copying the assignment prompt your professor gave you — it's a comprehension document you create with Claude after digesting the assignment requirements together, in your own words — explaining what the assignment actually asks for, which concepts it involves, which files are relevant, and where you think the key challenges are. Send the assignment description to Claude, tell it you want to generate such a document, have it create an Artifact, and Add to Project.

---

### Phase 3: Dynamic Learning and Progress Management

With the knowledge environment set up, the real learning begins. The core mechanism for this phase is maintaining a file called `progress.md`.

`progress.md` is a Markdown document stored in the Knowledge Base that records your learning state: which chapter you're currently on, which concepts you've mastered, which questions are still unresolved, where you left off last session. Its purpose is to give AI cross-conversation memory — because each time you start a new conversation, AI doesn't know what you discussed last time by default. But if you tell it "read `progress.md` first at the start of each conversation," it can immediately pick up where you left off without you re-explaining the context.

You need to add these two rules to your Instructions: at the start of each conversation, proactively read `progress.md` to understand current learning progress and unresolved issues from last time; whenever you say "that's it for today" or "ending study session," generate an updated `progress.md` (as an Artifact) recording what you learned today, your level of understanding, and what's still unclear, and remind you to Add to Project to replace the old version.

The actual learning conversation flow becomes very natural. You open the Project, start a new conversation, and say something like "continuing *Linear Algebra and Its Applications*, starting from matrix multiplication in Chapter 3." Claude reads progress.md, knows where you left off, and starts teaching. You ask questions, it explains, you're still confused, it tries another angle with a different example, you suddenly get it — this kind of dense interactive feedback is something no textbook or online course can provide.

During your learning sessions, whenever you feel you've truly understood a concept, ask Claude to help you write it up as an Artifact note, using your own words and the examples you discussed. Add that note to Project. By the end of a semester, your Knowledge Base contains not just your professor's materials, but an ever-growing collection of your own learning notes — each one a crystallization of your real understanding.

---

## 👨‍🏫 A Note from Your Instructor: Learning Hasn't Changed, But Speed and Depth Have

After building this system, you might ask a very direct question: How is this different from just having AI do my homework for me?

I want to answer this seriously, because the distinction is crucial.

When you truly understand matrix multiplication, you can do 100 practice problems in different forms, and for each one you can tell whether you got it right. When you don't understand and just had AI write it for you, nothing actually happened in your brain — AI understood it, not you. This method is designed so that: AI is responsible for explaining, giving examples, asking questions, and correcting errors; you are responsible for understanding, judging, and expressing. Homework is the stage where you demonstrate how much you've understood, not something you "get" from AI.

But I want to share something beyond just this principle, because you've probably heard "don't let AI think for you" before. Here's what I really want to say: **this method makes learning itself a fundamentally different experience.**

Traditional learning works like this: you read the book, don't understand a derivation, flip to the notes in the margin, still don't get it, search YouTube videos, spend half an hour and can't find one that addresses exactly where you're stuck, so you just memorize it, kind of remember it for the exam, forget it all afterward. In this process, feedback is scarce and frustration is cheap.

The new way: when you hit something you don't understand, just ask. AI knows which chapter you're studying, knows what your foundation level is, knows where you got stuck last time, and its explanation isn't a one-size-fits-all standard answer — it's designed specifically for your current state. This density of personalized feedback, in the pre-AI era, was available only to students who could afford private tutors.

Finally, here's something about this era. In the past, learning speed was limited by two bottlenecks: first, how good a teacher you had access to; second, how much time you could spend actively studying in the library. The first bottleneck has basically disappeared — the AI you now have access to has broader knowledge than any professor, infinite patience, and is available 24/7. The second bottleneck remains, but every minute of study time is now dramatically more efficient.

What's truly scarce now is your judgment — your ability to judge whether AI's explanation actually made things clear, whether you've genuinely understood, whether your assignment approach is going off track. This judgment is something AI can't give you, and it's exactly what this methodology aims to protect and develop.

---

## ✅ Completion Checklist

- [X] Created a Claude Project specifically for one course, with a clear name
- [X] Textbook has been split by chapter and compressed, uploaded to Knowledge Base
- [X] All course materials uploaded, file names organized clearly
- [X] Materials index document created and Added to Project
- [X] Instructions written, including role definition, index lookup rules, and progress.md maintenance rules
- [X] Requirements document created based on current assignment and Added to Project
- [ ] Completed at least one learning conversation, verified AI can read textbook and guide learning properly
- [ ] Updated and saved the first progress.md to Knowledge Base
- [ ] At least one personal learning note Artifact has been Added to Project

## 💡 Key Takeaways

The core of this method isn't technology — it's a new learning workflow. Organizing and uploading your textbook and materials creates the conditions for AI to work effectively; writing Instructions defines how your AI tutor operates; maintaining progress.md gives AI cross-conversation memory; writing your understanding as Artifact notes preserves the thinking AI helped you develop as something that truly belongs to you.

The setup cost is one-time. The benefits last the entire semester.
