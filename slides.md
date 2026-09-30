---
theme: default
colorSchema: dark
title: Your Backoffice, on Autopilot.
titleTemplate: '%s - OIBC AI Workshop'
info: |
  Session 2: Agentic AI for Small Businesses
highlighter: shiki
lineNumbers: false
drawings:
  persist: false
transition: slide-left
fonts:
  sans: 'Inter'
  mono: 'Fira Code'
---

<div class="flex flex-col items-center justify-center h-full text-center relative">
  <div class="text-xs uppercase tracking-[0.2em] mb-6 font-mono" style="color: rgba(255,255,255,0.35);">
    OIBC · AI Workshop · Session 2
  </div>
  <h1 class="text-6xl font-extrabold leading-tight mb-6" style="background: linear-gradient(to right, #60a5fa, #a855f7, #ec4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">
    Your Backoffice,<br/>on Autopilot.
  </h1>
  <p style="color: rgba(255,255,255,0.45); font-size: 1.1rem; max-width: 480px; line-height: 1.7; margin-bottom: 2rem;">
    Session 1 was about AI that answers.<br/>
    Today is about AI that <strong style="color: white;">does things</strong>.
  </p>
  <div class="flex gap-8 text-sm items-center" style="color: rgba(255,255,255,0.4);">
    <span class="flex items-center gap-2"><carbon-machine-learning class="w-4 h-4" /> Understand</span>
    <span style="color: rgba(255,255,255,0.15)">·</span>
    <span class="flex items-center gap-2"><carbon-tools class="w-4 h-4" /> See It Built</span>
    <span style="color: rgba(255,255,255,0.15)">·</span>
    <span class="flex items-center gap-2"><carbon-compare class="w-4 h-4" /> Compare</span>
    <span style="color: rgba(255,255,255,0.15)">·</span>
    <span class="flex items-center gap-2"><carbon-rocket class="w-4 h-4" /> Decide</span>
  </div>
  <div class="absolute bottom-8 left-0 right-0 flex justify-center">
    <div style="width: 200px; height: 1px; background: linear-gradient(to right, transparent, rgba(168,85,247,0.5), transparent);"></div>
  </div>
</div>

<!--
Welcome everyone. Last session covered what Gen AI is - ChatGPT, writing assistants, tools that answer your questions. Today is different. Today we talk about AI that doesn't wait to be asked. It watches, decides, and acts on your behalf.
-->

---
layout: default
---

# Today's Agenda

<div class="grid grid-cols-2 gap-4 mt-6">
  <div style="background: rgba(59,130,246,0.07); border: 1px solid rgba(59,130,246,0.25); border-radius: 16px; padding: 1.25rem;">
    <div style="color: #60a5fa; font-family: monospace; font-size: 0.7rem; text-transform: uppercase; letter-spacing: 0.15em; margin-bottom: 0.75rem;">Part 1 · Foundations</div>
    <ul style="color: #d1d5db; font-size: 0.9rem; list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.5rem;">
      <li class="flex items-center gap-2"><carbon-flash class="w-4 h-4 text-blue-400 flex-shrink-0" /> From Gen AI to Agentic AI</li>
      <li class="flex items-center gap-2"><carbon-chat-bot class="w-4 h-4 text-blue-400 flex-shrink-0" /> What is an AI Agent?</li>
      <li class="flex items-center gap-2"><carbon-compare class="w-4 h-4 text-blue-400 flex-shrink-0" /> Tools available today</li>
    </ul>
  </div>
  <div style="background: rgba(168,85,247,0.07); border: 1px solid rgba(168,85,247,0.25); border-radius: 16px; padding: 1.25rem;">
    <div style="color: #c084fc; font-family: monospace; font-size: 0.7rem; text-transform: uppercase; letter-spacing: 0.15em; margin-bottom: 0.75rem;">Part 2 · Business Problems</div>
    <ul style="color: #d1d5db; font-size: 0.9rem; list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.5rem;">
      <li class="flex items-center gap-2"><carbon-portfolio class="w-4 h-4 text-purple-400 flex-shrink-0" /> Real agents, real businesses</li>
      <li class="flex items-center gap-2"><carbon-search class="w-4 h-4 text-purple-400 flex-shrink-0" /> What makes a good agent use case</li>
    </ul>
  </div>
  <div style="background: rgba(236,72,153,0.07); border: 1px solid rgba(236,72,153,0.25); border-radius: 16px; padding: 1.25rem;">
    <div style="color: #f472b6; font-family: monospace; font-size: 0.7rem; text-transform: uppercase; letter-spacing: 0.15em; margin-bottom: 0.75rem;">Part 3 · Key Concepts</div>
    <ul style="color: #d1d5db; font-size: 0.9rem; list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.5rem;">
      <li class="flex items-center gap-2"><carbon-idea class="w-4 h-4 text-pink-400 flex-shrink-0" /> OpenAI · Anthropic · API keys</li>
      <li class="flex items-center gap-2"><carbon-plug class="w-4 h-4 text-pink-400 flex-shrink-0" /> Connectors · Skills · MCP · HITL</li>
    </ul>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.1); border-radius: 16px; padding: 1.25rem;">
    <div style="color: #9ca3af; font-family: monospace; font-size: 0.7rem; text-transform: uppercase; letter-spacing: 0.15em; margin-bottom: 0.75rem;">Part 4 · Live Build</div>
    <ul style="color: #d1d5db; font-size: 0.9rem; list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.5rem;">
      <li class="flex items-center gap-2"><carbon-tools class="w-4 h-4 text-gray-400 flex-shrink-0" /> Build it in OpenClaw + Setod</li>
      <li class="flex items-center gap-2"><carbon-chemistry class="w-4 h-4 text-gray-400 flex-shrink-0" /> Test, break, and improve</li>
    </ul>
  </div>
</div>

---
layout: section
---

<div class="text-center">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1rem;">Part 1</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; background: linear-gradient(to right, #60a5fa, #a855f7, #ec4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; line-height: 1.1;">From Gen AI<br/>to Agentic AI</h1>
</div>

---
layout: default
---

# Where We Left Off

<div style="margin: 1.5rem auto 0; max-width: 700px; display: flex; flex-direction: column; gap: 1rem;">
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.1rem 1.5rem; font-size: 0.85rem; color: #9ca3af;">
    <span style="font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; font-size: 0.65rem; color: rgba(255,255,255,0.25);">Session 1 covered</span><br/>
    ChatGPT, Claude, Canva AI · Prompting · Zapier / n8n · The 4 business problems · 24 real businesses
  </div>
  <div class="grid grid-cols-2 gap-4">
    <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.1); border-radius: 18px; padding: 1.75rem; text-align: center;">
      <carbon-chat class="w-10 h-10 mx-auto mb-3" style="color: #6b7280;" />
      <div style="font-weight: 700; font-size: 1rem; color: #9ca3af; margin-bottom: 0.75rem;">Gen AI - what you learned</div>
      <div style="font-size: 0.85rem; color: #6b7280; line-height: 1.8;">
        You open ChatGPT<br/>
        You type a question<br/>
        It answers<br/>
        <strong style="color: #9ca3af;">You still do the work</strong>
      </div>
    </div>
    <div style="background: rgba(99,102,241,0.08); border: 1px solid rgba(168,85,247,0.4); border-radius: 18px; padding: 1.75rem; text-align: center; box-shadow: 0 0 40px rgba(168,85,247,0.1);">
      <carbon-machine-learning class="w-10 h-10 mx-auto mb-3" style="color: #a855f7;" />
      <div style="font-weight: 700; font-size: 1rem; margin-bottom: 0.75rem; background: linear-gradient(to right, #60a5fa, #a855f7); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">Agentic AI - today</div>
      <div style="font-size: 0.85rem; color: #d1d5db; line-height: 1.8;">
        You set a goal once<br/>
        Something happens in your business<br/>
        It understands and decides<br/>
        <strong style="color: white;">It acts - without being asked</strong>
      </div>
    </div>
  </div>
  <div style="background: rgba(251,191,36,0.06); border: 1px solid rgba(251,191,36,0.2); border-radius: 14px; padding: 1rem 1.5rem; font-size: 0.9rem; color: #fbbf24; text-align: center;">
    Remember the <strong>Scale Up 🚀</strong> problem from last session?<br/>
    <span style="color: rgba(255,255,255,0.5); font-size: 0.8rem;">AI Agents are the answer to "I can't grow without hiring more people."</span>
  </div>
</div>

<!--
They already know ChatGPT. They already tried prompting. They already saw Zapier and n8n. Today we go one level up - AI that doesn't wait to be asked.
-->

---
layout: default
---

# Four Levels - The Difference That Matters

<div class="grid grid-cols-4 gap-3 mt-8">
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 16px; padding: 1.25rem; text-align: center;">
    <carbon-chat class="w-10 h-10 mx-auto mb-3" style="color: #9ca3af;" />
    <div style="font-weight: 700; font-size: 1rem; color: #e5e7eb; margin-bottom: 0.5rem;">Chatbot</div>
    <div style="font-size: 0.6rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: #4b5563; margin-bottom: 0.75rem;">ChatGPT</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #9ca3af;">You open it · You ask</div>
    <div style="color: rgba(255,255,255,0.2); margin: 0.35rem 0;">↓</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #9ca3af;">It answers</div>
    <div style="margin-top: 0.85rem; font-size: 0.7rem; color: #4b5563;">You initiate every time</div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 16px; padding: 1.25rem; text-align: center;">
    <carbon-settings class="w-10 h-10 mx-auto mb-3" style="color: #9ca3af;" />
    <div style="font-weight: 700; font-size: 1rem; color: #e5e7eb; margin-bottom: 0.5rem;">Automation</div>
    <div style="font-size: 0.6rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: #4b5563; margin-bottom: 0.75rem;">Zapier, Make, n8n</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #9ca3af;">If X happens</div>
    <div style="color: rgba(255,255,255,0.2); margin: 0.35rem 0;">↓</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #9ca3af;">Do Y - always</div>
    <div style="margin-top: 0.85rem; font-size: 0.7rem; color: #4b5563;">Every rule must be pre-written</div>
  </div>
  <div style="background: rgba(99,102,241,0.08); border: 1px solid rgba(168,85,247,0.4); border-radius: 16px; padding: 1.25rem; text-align: center; box-shadow: 0 0 30px rgba(168,85,247,0.1);">
    <carbon-flash class="w-10 h-10 mx-auto mb-3" style="color: #a855f7;" />
    <div style="font-weight: 700; font-size: 1rem; margin-bottom: 0.5rem; background: linear-gradient(to right, #60a5fa, #a855f7); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">AI in Agent Mode</div>
    <div style="font-size: 0.6rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: #7c3aed; margin-bottom: 0.75rem;">ChatGPT Work · Claude Projects</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #d1d5db;">You describe a goal</div>
    <div style="color: #a855f7; margin: 0.35rem 0;">↓</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #d1d5db;">It works through steps</div>
    <div style="color: #a855f7; margin: 0.35rem 0;">↓</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #d1d5db;">Returns a finished result</div>
  </div>
  <div style="background: rgba(251,191,36,0.06); border: 1px solid rgba(251,191,36,0.3); border-radius: 16px; padding: 1.25rem; text-align: center;">
    <carbon-machine-learning class="w-10 h-10 mx-auto mb-3" style="color: #fbbf24;" />
    <div style="font-weight: 700; font-size: 1rem; color: #fde68a; margin-bottom: 0.5rem;">Dedicated Agent</div>
    <div style="font-size: 0.6rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: #92400e; margin-bottom: 0.75rem;">OpenClaw · Setod - Today ↑</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #d1d5db;">Give it a goal once</div>
    <div style="color: #fbbf24; margin: 0.3rem 0;">↓</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #d1d5db;">Watches in background</div>
    <div style="color: #fbbf24; margin: 0.3rem 0;">↓</div>
    <div style="font-size: 0.75rem; font-family: monospace; color: #d1d5db;">Acts without being asked</div>
  </div>
</div>

---
layout: default
---

# The Agent Framework

<div class="flex items-center justify-center mt-10 gap-0">
  <div style="text-align: center; padding: 0 1.5rem;">
    <div style="width: 80px; height: 80px; border-radius: 50%; background: rgba(59,130,246,0.15); border: 2px solid rgba(59,130,246,0.5); display: flex; align-items: center; justify-content: center; margin: 0 auto 0.75rem; box-shadow: 0 0 20px rgba(59,130,246,0.2);">
      <carbon-flash style="color: #60a5fa; font-size: 2rem;" />
    </div>
    <div style="font-weight: 700; color: #60a5fa;">Trigger</div>
    <div style="font-size: 0.75rem; color: rgba(255,255,255,0.35); margin-top: 0.25rem;">Something happens</div>
  </div>
  <div style="font-size: 1.5rem; color: rgba(255,255,255,0.15); padding-bottom: 2rem;">→</div>
  <div style="text-align: center; padding: 0 1.5rem;">
    <div style="width: 80px; height: 80px; border-radius: 50%; background: rgba(168,85,247,0.15); border: 2px solid rgba(168,85,247,0.5); display: flex; align-items: center; justify-content: center; margin: 0 auto 0.75rem; box-shadow: 0 0 20px rgba(168,85,247,0.2);">
      <carbon-machine-learning style="color: #a855f7; font-size: 2rem;" />
    </div>
    <div style="font-weight: 700; color: #c084fc;">Understand</div>
    <div style="font-size: 0.75rem; color: rgba(255,255,255,0.35); margin-top: 0.25rem;">What does it mean?</div>
  </div>
  <div style="font-size: 1.5rem; color: rgba(255,255,255,0.15); padding-bottom: 2rem;">→</div>
  <div style="text-align: center; padding: 0 1.5rem;">
    <div style="width: 80px; height: 80px; border-radius: 50%; background: rgba(236,72,153,0.15); border: 2px solid rgba(236,72,153,0.5); display: flex; align-items: center; justify-content: center; margin: 0 auto 0.75rem; box-shadow: 0 0 20px rgba(236,72,153,0.2);">
      <carbon-decision-tree style="color: #ec4899; font-size: 2rem;" />
    </div>
    <div style="font-weight: 700; color: #f472b6;">Decide</div>
    <div style="font-size: 0.75rem; color: rgba(255,255,255,0.35); margin-top: 0.25rem;">What should happen?</div>
  </div>
  <div style="font-size: 1.5rem; color: rgba(255,255,255,0.15); padding-bottom: 2rem;">→</div>
  <div style="text-align: center; padding: 0 1.5rem;">
    <div style="width: 80px; height: 80px; border-radius: 50%; background: rgba(16,185,129,0.15); border: 2px solid rgba(16,185,129,0.5); display: flex; align-items: center; justify-content: center; margin: 0 auto 0.75rem; box-shadow: 0 0 20px rgba(16,185,129,0.2);">
      <carbon-send style="color: #34d399; font-size: 2rem;" />
    </div>
    <div style="font-weight: 700; color: #34d399;">Act</div>
    <div style="font-size: 0.75rem; color: rgba(255,255,255,0.35); margin-top: 0.25rem;">Do something real</div>
  </div>
</div>
<div class="mt-10 text-center" style="max-width: 600px; margin: 2.5rem auto 0;">
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.25rem; font-size: 0.9rem; color: #9ca3af;">
    New message arrives →
    <span style="color: #c084fc;">Is this urgent?</span> →
    <span style="color: #f472b6;">Yes - property damage risk</span> →
    <span style="color: #34d399;">Alert you immediately</span>
  </div>
</div>

---
layout: default
---

# Tools Available Today

  <div style="overflow-x: auto; margin-top: 1.5rem;">
<table style="width: 100%; border-collapse: separate; border-spacing: 0; font-size: 0.88rem;">
  <thead>
    <tr>
      <th style="text-align: left; padding: 0.75rem 1rem; color: rgba(255,255,255,0.4); font-weight: 500; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; border-bottom: 1px solid rgba(255,255,255,0.08);">Tool</th>
      <th style="text-align: left; padding: 0.75rem 1rem; color: rgba(255,255,255,0.4); font-weight: 500; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; border-bottom: 1px solid rgba(255,255,255,0.08);">Best for</th>
      <th style="text-align: left; padding: 0.75rem 1rem; color: rgba(255,255,255,0.4); font-weight: 500; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; border-bottom: 1px solid rgba(255,255,255,0.08);">How it works</th>
      <th style="text-align: left; padding: 0.75rem 1rem; color: rgba(255,255,255,0.4); font-weight: 500; font-size: 0.75rem; text-transform: uppercase; letter-spacing: 0.1em; border-bottom: 1px solid rgba(255,255,255,0.08);">Technical skill</th>
    </tr>
  </thead>
  <tbody>
    <tr style="background: rgba(255,255,255,0.02);">
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);">
        <span style="color: #e5e7eb; font-weight: 600;">Zapier · Make</span>
        <span style="display: block; font-size: 0.65rem; font-family: monospace; color: #4b5563; margin-top: 0.2rem;">from Session 1</span>
      </td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Simple app-to-app triggers</td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">If X → do Y, always</td>
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);"><span style="color: #34d399;">Low</span></td>
    </tr>
    <tr style="background: rgba(255,255,255,0.02);">
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);">
        <span style="color: #e5e7eb; font-weight: 600;">n8n</span>
        <span style="display: block; font-size: 0.65rem; font-family: monospace; color: #4b5563; margin-top: 0.2rem;">from Session 1</span>
      </td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Complex workflows, self-hosted</td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Visual flow builder</td>
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);"><span style="color: #fbbf24;">Medium</span></td>
    </tr>
    <tr style="background: rgba(255,255,255,0.02);">
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);">
        <span style="color: #e5e7eb; font-weight: 600;">ChatGPT Work</span>
        <span style="display: block; font-size: 0.65rem; font-family: monospace; color: #4b5563; margin-top: 0.2rem;">Claude Projects</span>
      </td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Familiar tools, task-based agents</td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Describe task, connect apps</td>
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);"><span style="color: #34d399;">Low</span></td>
    </tr>
    <tr style="background: rgba(168,85,247,0.06); border: 1px solid rgba(168,85,247,0.2);">
      <td style="padding: 0.9rem 1rem; color: #e5e7eb; font-weight: 600; border-bottom: 1px solid rgba(255,255,255,0.05);">OpenClaw</td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Fully custom agents, self-hosted</td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Code + configuration</td>
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);"><span style="color: #f87171;">High</span></td>
    </tr>
    <tr style="background: rgba(255,255,255,0.02);">
      <td style="padding: 0.9rem 1rem; color: #e5e7eb; font-weight: 600; border-bottom: 1px solid rgba(255,255,255,0.05);">Setod</td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Built for this workshop</td>
      <td style="padding: 0.9rem 1rem; color: #9ca3af; border-bottom: 1px solid rgba(255,255,255,0.05);">Plain English instructions</td>
      <td style="padding: 0.9rem 1rem; border-bottom: 1px solid rgba(255,255,255,0.05);"><span style="color: #34d399;">None</span></td>
    </tr>
  </tbody>
</table>
</div>
<div style="margin-top: 1.25rem; text-align: center; color: #9ca3af; font-size: 0.9rem;">
  Today we'll go deeper on agents - showing you <span style="color: white; font-weight: 600;">OpenClaw</span> and <span style="color: white; font-weight: 600;">Setod</span> to demonstrate the concepts.
</div>

<!--
No tool is wrong here. The question is: what fits your time, your budget, and your comfort with technology. We're going to show you two ends of the spectrum today.
-->

---
layout: section
---

<div class="text-center">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1rem;">Part 2</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; background: linear-gradient(to right, #a855f7, #ec4899, #f87171); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; line-height: 1.1;">Real Problems,<br/>Real Agents</h1>
  <p style="color: rgba(255,255,255,0.4); margin-top: 1rem; font-size: 1rem;">What agents actually look like when they're running</p>
</div>

---
layout: default
---

# Agents Already Running in the Wild

<div class="grid grid-cols-3 gap-4 mt-5" style="max-width: 900px; margin: 1.25rem auto 0;">
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <div style="width: 28px; height: 28px; border-radius: 7px; background: rgba(236,72,153,0.15); border: 1px solid rgba(236,72,153,0.3); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-chat class="w-3 h-3" style="color: #ec4899;" />
      </div>
      <div style="font-weight: 600; color: #e5e7eb; font-size: 0.82rem;">Instagram Assistant</div>
    </div>
    <div style="font-size: 0.75rem; color: #6b7280; line-height: 1.6;">Comment arrives → evaluate tone → delete if insulting or offensive</div>
    <div class="flex items-center gap-1" style="margin-top: 0.65rem; font-size: 0.6rem; font-family: monospace; color: #4b5563;"><carbon-chat class="w-3 h-3" style="color: #4b5563;" /> On message · Instagram</div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <div style="width: 28px; height: 28px; border-radius: 7px; background: rgba(251,191,36,0.15); border: 1px solid rgba(251,191,36,0.3); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-notification class="w-3 h-3" style="color: #fbbf24;" />
      </div>
      <div style="font-weight: 600; color: #e5e7eb; font-size: 0.82rem;">Telegram Lead Finder</div>
    </div>
    <div style="font-size: 0.75rem; color: #6b7280; line-height: 1.6;">Monitor group chats for catering leads → send SMS alert when found</div>
    <div class="flex items-center gap-1" style="margin-top: 0.65rem; font-size: 0.6rem; font-family: monospace; color: #4b5563;"><carbon-time class="w-3 h-3" style="color: #4b5563;" /> Scheduled · Telegram · SMS</div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <div style="width: 28px; height: 28px; border-radius: 7px; background: rgba(168,85,247,0.15); border: 1px solid rgba(168,85,247,0.3); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-search class="w-3 h-3" style="color: #a855f7;" />
      </div>
      <div style="font-weight: 600; color: #e5e7eb; font-size: 0.82rem;">Canadian Tender Sniper</div>
    </div>
    <div style="font-size: 0.75rem; color: #6b7280; line-height: 1.6;">Monitor CanadaBuys for new construction tenders → alert when found</div>
    <div class="flex items-center gap-1" style="margin-top: 0.65rem; font-size: 0.6rem; font-family: monospace; color: #4b5563;"><carbon-time class="w-3 h-3" style="color: #4b5563;" /> Scheduled · Web · SMS</div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <div style="width: 28px; height: 28px; border-radius: 7px; background: rgba(59,130,246,0.15); border: 1px solid rgba(59,130,246,0.3); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-calendar class="w-3 h-3" style="color: #60a5fa;" />
      </div>
      <div style="font-weight: 600; color: #e5e7eb; font-size: 0.82rem;">Cancellation &amp; Waitlist</div>
    </div>
    <div style="font-size: 0.75rem; color: #6b7280; line-height: 1.6;">Cancellation arrives → update calendar → notify next person on waiting list</div>
    <div class="flex items-center gap-1" style="margin-top: 0.65rem; font-size: 0.6rem; font-family: monospace; color: #4b5563;"><carbon-chat class="w-3 h-3" style="color: #4b5563;" /> On message · Calendar · SMS</div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <div style="width: 28px; height: 28px; border-radius: 7px; background: rgba(59,130,246,0.15); border: 1px solid rgba(59,130,246,0.3); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-alarm class="w-3 h-3" style="color: #60a5fa;" />
      </div>
      <div style="font-weight: 600; color: #e5e7eb; font-size: 0.82rem;">Meeting SMS Reminder</div>
    </div>
    <div style="font-size: 0.75rem; color: #6b7280; line-height: 1.6;">Check calendar for meetings in next 2 hours → send SMS reminder</div>
    <div class="flex items-center gap-1" style="margin-top: 0.65rem; font-size: 0.6rem; font-family: monospace; color: #4b5563;"><carbon-time class="w-3 h-3" style="color: #4b5563;" /> Scheduled · Google Calendar · SMS</div>
  </div>
  <div style="background: rgba(239,68,68,0.05); border: 1px solid rgba(239,68,68,0.25); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <div style="width: 28px; height: 28px; border-radius: 7px; background: rgba(239,68,68,0.15); border: 1px solid rgba(239,68,68,0.3); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-email class="w-3 h-3" style="color: #f87171;" />
      </div>
      <div style="font-weight: 600; color: #e5e7eb; font-size: 0.82rem;">Emergency Email Triage</div>
    </div>
    <div style="font-size: 0.75rem; color: #6b7280; line-height: 1.6;">Read inbox → classify urgency → alert if emergency, queue if not</div>
    <div class="flex items-center gap-1" style="margin-top: 0.65rem; font-size: 0.6rem; font-family: monospace; color: #4b5563;"><carbon-time class="w-3 h-3" style="color: #4b5563;" /> Scheduled · Gmail · SMS</div>
  </div>
</div>

---
layout: default
---

# What Makes a Good Agent Use Case?

<div class="grid grid-cols-2 gap-5 mt-6" style="max-width: 760px; margin: 1.5rem auto 0;">
  <div style="background: rgba(52,211,153,0.06); border: 1px solid rgba(52,211,153,0.2); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #34d399; margin-bottom: 1rem;">Good fit ✓</div>
    <ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.85rem;">
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        Happens repeatedly - daily, weekly, on every message
      </li>
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        Requires reading and understanding something
      </li>
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        Has a clear action when the condition is met
      </li>
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        Missing it has a real cost (lost lead, delayed response)
      </li>
    </ul>
  </div>
  <div style="background: rgba(239,68,68,0.05); border: 1px solid rgba(239,68,68,0.15); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #f87171; margin-bottom: 1rem;">Not ready yet ✗</div>
    <ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.85rem;">
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        Happens once or unpredictably
      </li>
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        Requires judgment you can't describe in words
      </li>
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        A mistake would seriously damage trust
      </li>
      <li class="flex items-start gap-3" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        Requires relationships or negotiation
      </li>
    </ul>
  </div>
</div>
<div style="margin-top: 1.5rem; text-align: center; color: #9ca3af; font-size: 0.9rem; max-width: 600px; margin-left: auto; margin-right: auto;">
  The clearest signal: if you can write down exactly what you'd do when X happens - an agent can do it for you.
</div>

---
layout: section
---

<div class="text-center">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1rem;">Part 3</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; background: linear-gradient(to right, #ec4899, #a855f7, #60a5fa); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; line-height: 1.1;">Before We Build ;<br/>Key Concepts</h1>
  <p style="color: rgba(255,255,255,0.4); margin-top: 1rem; font-size: 1rem;">Everything you need to follow the live build</p>
</div>

---
layout: default
---

# The Brains ( Models ) - OpenAI & Anthropic

<div class="grid grid-cols-2 gap-6 mt-6" style="max-width: 760px; margin: 1.25rem auto 0;">
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 18px; padding: 1.75rem; text-align: center;">
    <img src="/openai.svg" style="width: 52px; height: 52px; margin: 0 auto 0.75rem; display: block; filter: invert(1);" />
    <div style="font-weight: 700; font-size: 1.1rem; color: #e5e7eb; margin-bottom: 0.5rem;">OpenAI</div>
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: #4b5563; margin-bottom: 0.75rem;">GPT-4o · GPT-5 · ChatGPT</div>
    <div style="font-size: 0.85rem; color: #9ca3af; line-height: 1.7;">The company behind ChatGPT. Their models power millions of agents worldwide.</div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 18px; padding: 1.75rem; text-align: center;">
    <img src="/anthropic.svg" style="width: 52px; height: 52px; margin: 0 auto 0.75rem; display: block;" />
    <div style="font-weight: 700; font-size: 1.1rem; color: #e5e7eb; margin-bottom: 0.5rem;">Anthropic</div>
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: #4b5563; margin-bottom: 0.75rem;">Claude 3.5 · Claude 4</div>
    <div style="font-size: 0.85rem; color: #9ca3af; line-height: 1.7;">OpenAI's main competitor. Known for following instructions carefully - great for agents.</div>
  </div>
</div>
<div style="max-width: 760px; margin: 1.25rem auto 0; background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.25rem 1.5rem;">
  <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: rgba(255,255,255,0.3); margin-bottom: 0.75rem;">How to think about it</div>
  <div class="grid grid-cols-3 gap-4" style="font-size: 0.85rem; text-align: center;">
    <div>
      <div style="color: #60a5fa; font-weight: 600; margin-bottom: 0.25rem;">OpenClaw</div>
      <div style="color: #6b7280;">The platform - the car</div>
    </div>
    <div style="color: rgba(255,255,255,0.15); font-size: 1.5rem; display: flex; align-items: center; justify-content: center;">+</div>
    <div>
      <div style="color: #a855f7; font-weight: 600; margin-bottom: 0.25rem;">OpenAI / Anthropic</div>
      <div style="color: #6b7280;">The engine inside it</div>
    </div>
  </div>
</div>

---
layout: default
---

# API Keys & BYOK

<div style="max-width: 720px; margin: 1.5rem auto 0; display: flex; flex-direction: column; gap: 1rem;">
  <div style="background: rgba(251,191,36,0.06); border: 1px solid rgba(251,191,36,0.25); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #fbbf24; margin-bottom: 0.75rem;">What is an API Key?</div>
    <div style="font-size: 0.95rem; color: #e5e7eb; line-height: 1.8;">
      Think of it as a <strong style="color: white;">personal password</strong> that lets your agent use OpenAI or Anthropic's model.<br/>
      <span style="color: #9ca3af; font-size: 0.85rem;">You generate it once on their website. You paste it into Setod. That's it.</span>
    </div>
  </div>
  <div style="background: rgba(59,130,246,0.06); border: 1px solid rgba(59,130,246,0.2); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #60a5fa; margin-bottom: 0.75rem;">BYOK - Bring Your Own Key</div>
    <div style="font-size: 0.9rem; color: #d1d5db; line-height: 1.8;">
      Platforms in this model doesn't charge you for AI usage - you pay OpenAI or Anthropic directly.<br/>
      <span style="color: #9ca3af; font-size: 0.85rem;">This means: <strong style="color: white;">your data never passes through the platform's billing</strong>. You control your costs.</span>
    </div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.25rem 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: rgba(255,255,255,0.3); margin-bottom: 0.75rem;">How to get one (2 minutes)</div>
    <div class="flex items-start gap-4" style="font-size: 0.85rem; color: #9ca3af;">
      <div class="flex items-start gap-2"><span style="color: #60a5fa; font-weight: 700; flex-shrink: 0;">1.</span> platform.openai.com → API Keys → Create new</div>
      <div style="color: rgba(255,255,255,0.1);">·</div>
      <div class="flex items-start gap-2"><span style="color: #60a5fa; font-weight: 700; flex-shrink: 0;">2.</span> Copy the key</div>
      <div style="color: rgba(255,255,255,0.1);">·</div>
      <div class="flex items-start gap-2"><span style="color: #60a5fa; font-weight: 700; flex-shrink: 0;">3.</span> Paste into the settings</div>
    </div>
  </div>
</div>

---
layout: default
---

# Connectors, Skills & Instructions

<div style="max-width: 720px; margin: 1.5rem auto 0; display: flex; flex-direction: column; gap: 0.85rem;">
  <div class="flex items-start gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <carbon-plug class="w-7 h-7 flex-shrink-0 mt-0.5" style="color: #60a5fa;" />
    <div>
      <div style="font-weight: 600; color: #60a5fa; margin-bottom: 0.25rem;">Connectors</div>
      <div style="font-size: 0.85rem; color: #9ca3af; line-height: 1.6;">The integrations that let your agent see and act on the outside world - Gmail, Telegram, SMS, Google Calendar, Instagram. Connect them with a few clicks using OAuth or an API key. No code.</div>
    </div>
  </div>
  <div class="flex items-start gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <carbon-document class="w-7 h-7 flex-shrink-0 mt-0.5" style="color: #a855f7;" />
    <div>
      <div style="font-weight: 600; color: #a855f7; margin-bottom: 0.25rem;">Instructions</div>
      <div style="font-size: 0.85rem; color: #9ca3af; line-height: 1.6;">The plain-English rules you write that tell the agent how to behave. "If the message describes flooding, fire, or electrical hazard - send me an SMS." This is your logic.</div>
    </div>
  </div>
  <div class="flex items-start gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1.1rem 1.25rem;">
    <carbon-tools class="w-7 h-7 flex-shrink-0 mt-0.5" style="color: #ec4899;" />
    <div>
      <div style="font-weight: 600; color: #ec4899; margin-bottom: 0.25rem;">Skills</div>
      <div style="font-size: 0.85rem; color: #9ca3af; line-height: 1.6;">Reusable instruction sets - most are ready to use, built by others in the community. You can also create your own if needed. Apply them across agents to keep behaviour consistent.</div>
    </div>
  </div>
</div>

---
layout: default
---

# Two Terms Worth Knowing

<div class="grid grid-cols-2 gap-6 mt-6" style="max-width: 760px; margin: 1.25rem auto 0;">
  <div style="background: rgba(168,85,247,0.07); border: 1px solid rgba(168,85,247,0.25); border-radius: 18px; padding: 2rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #a855f7; margin-bottom: 1rem;">HITL · Human in the Loop</div>
    <carbon-user-activity style="font-size: 2rem; color: #a855f7; display: block; margin-bottom: 1rem;" />
    <div style="font-size: 0.9rem; color: #d1d5db; line-height: 1.8; margin-bottom: 1rem;">
      Before the agent sends, deletes, or posts - it stops and asks you to approve.
    </div>
    <div style="background: rgba(255,255,255,0.04); border-radius: 10px; padding: 0.85rem 1rem; font-size: 0.8rem; color: #9ca3af; font-family: monospace; line-height: 1.7;">
      Agent: "I'm about to send this reply to your customer. OK?"<br/>
      <span style="color: #34d399;">You: Approve → it sends</span><br/>
      <span style="color: #f87171;">You: Reject → it stops</span>
    </div>
    <div style="margin-top: 0.85rem; font-size: 0.75rem; color: #7c3aed;">Use this when mistakes are costly</div>
  </div>
  <div style="background: rgba(59,130,246,0.06); border: 1px solid rgba(59,130,246,0.2); border-radius: 18px; padding: 2rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #60a5fa; margin-bottom: 1rem;">MCP · Model Context Protocol</div>
    <img src="/mcp.svg" style="width: 48px; height: 48px; margin: 0 auto 1rem; display: block; filter: invert(1);" />
    <div style="font-size: 0.9rem; color: #d1d5db; line-height: 1.8; margin-bottom: 1rem;">
      A new open standard that lets AI models connect to any tool - databases, APIs, apps - in a universal way.
    </div>
    <div style="background: rgba(255,255,255,0.04); border-radius: 10px; padding: 0.85rem 1rem; font-size: 0.8rem; color: #9ca3af; line-height: 1.6;">
      Think of it as a USB-C port for AI - instead of each tool needing a custom integration, they all speak one language.
    </div>
    <div style="margin-top: 0.85rem; font-size: 0.75rem; color: #3b82f6;">Growing fast - just know the term for now</div>
  </div>
</div>

---
layout: section
---

<div class="text-center">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1rem;">Part 4</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; background: linear-gradient(to right, #f87171, #fb923c, #fbbf24); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; line-height: 1.1;">Emergency Message Agent</h1>
  <p style="color: rgba(255,255,255,0.4); margin-top: 1rem; font-size: 1rem;">The use case - then we build it two ways</p>
</div>

---
layout: default
---

# The Business Problem

<div style="margin-top: 1.5rem; border-left: 3px solid; border-image: linear-gradient(to bottom, #f87171, #fb923c) 1; padding: 1.5rem 2rem; background: rgba(248,113,113,0.05); border-radius: 0 16px 16px 0; max-width: 680px; margin-left: auto; margin-right: auto;">
  <p style="color: #e5e7eb; font-size: 1.1rem; line-height: 1.8; font-style: italic;">
    "I run a service business. I do not want to check messages all night.<br/><br/>
    But if a customer has a <strong style="color: #fb923c; font-style: normal;">real emergency</strong>, I cannot let that wait until morning."
  </p>
</div>
<div style="margin-top: 1.5rem; background: rgba(239,68,68,0.08); border: 1px solid rgba(239,68,68,0.3); border-radius: 14px; padding: 1.25rem 1.5rem; max-width: 680px; margin-left: auto; margin-right: auto;">
  <div class="flex items-center gap-2 mb-2">
    <carbon-alarm class="w-4 h-4" style="color: #f87171;" />
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #f87171;">Example Message</div>
  </div>
  <div style="color: #f3f4f6; font-size: 1rem;">"A pipe just burst in the basement and water is spreading everywhere."</div>
</div>
<div class="grid grid-cols-2 gap-4 mt-4" style="max-width: 680px; margin-left: auto; margin-right: auto;">
  <div style="background: rgba(239,68,68,0.06); border: 1px solid rgba(239,68,68,0.2); border-radius: 12px; padding: 1rem 1.25rem; font-size: 0.85rem;">
    <div style="color: #f87171; font-weight: 600; margin-bottom: 0.5rem;">🚨 Emergency - act now</div>
    <div style="color: #9ca3af; line-height: 1.8;">Burst pipe · Flooding · Electrical hazard · Security issue · Health risk</div>
  </div>
  <div style="background: rgba(16,185,129,0.05); border: 1px solid rgba(16,185,129,0.2); border-radius: 12px; padding: 1rem 1.25rem; font-size: 0.85rem;">
    <div style="color: #34d399; font-weight: 600; margin-bottom: 0.5rem;">✓ Not urgent - wait until morning</div>
    <div style="color: #9ca3af; line-height: 1.8;">Pricing request · Next-week booking · General questions</div>
  </div>
</div>
<div style="margin-top: 1.25rem; text-align: center; color: #9ca3af; font-size: 0.9rem;">
  The agent must <span style="color: white; font-weight: 600;">understand meaning</span> - not just search for keywords like "urgent."
</div>

---
layout: default
---

# 5 Concepts That Make an Agent

<div style="max-width: 650px; margin: 1.5rem auto 0; display: flex; flex-direction: column; gap: 0.75rem;">
  <div class="flex items-center gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1rem 1.25rem;">
    <carbon-chat-bot class="w-7 h-7 flex-shrink-0" style="color: #60a5fa;" />
    <div>
      <div style="font-weight: 600; color: #60a5fa;">Agent</div>
      <div style="font-size: 0.85rem; color: #9ca3af;">What is its job?</div>
    </div>
  </div>
  <div class="flex items-center gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1rem 1.25rem;">
    <carbon-document class="w-7 h-7 flex-shrink-0" style="color: #a855f7;" />
    <div>
      <div style="font-weight: 600; color: #a855f7;">Instructions</div>
      <div style="font-size: 0.85rem; color: #9ca3af;">What rules should it follow?</div>
    </div>
  </div>
  <div class="flex items-center gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1rem 1.25rem;">
    <carbon-email class="w-7 h-7 flex-shrink-0" style="color: #ec4899;" />
    <div>
      <div style="font-weight: 600; color: #ec4899;">Channel</div>
      <div style="font-size: 0.85rem; color: #9ca3af;">Where does information come in? (Email, Telegram, SMS…)</div>
    </div>
  </div>
  <div class="flex items-center gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1rem 1.25rem;">
    <carbon-tools class="w-7 h-7 flex-shrink-0" style="color: #34d399;" />
    <div>
      <div style="font-weight: 600; color: #34d399;">Tools</div>
      <div style="font-size: 0.85rem; color: #9ca3af;">What can it use? (Web search, calendar, database…)</div>
    </div>
  </div>
  <div class="flex items-center gap-4" style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 14px; padding: 1rem 1.25rem;">
    <carbon-send class="w-7 h-7 flex-shrink-0" style="color: #fb923c;" />
    <div>
      <div style="font-weight: 600; color: #fb923c;">Action</div>
      <div style="font-size: 0.85rem; color: #9ca3af;">What does it do after deciding? (Send alert, reply, log…)</div>
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

<div class="flex flex-col items-center justify-center h-full">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1.5rem;">Live Build - OpenClaw</div>
  <h2 style="font-size: 2.5rem; font-weight: 800; color: white; margin-bottom: 0.5rem;">Building in OpenClaw</h2>
  <p style="color: #9ca3af; font-size: 1rem; max-width: 500px; line-height: 1.7; margin-bottom: 2rem;">Open-source, self-hosted, fully customizable.<br/>Powerful - and we'll be honest about what that takes.</p>
  <div style="display: flex; flex-direction: column; gap: 1rem; max-width: 480px; width: 100%; text-align: left; margin-bottom: 2.5rem;">
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: rgba(168,85,247,0.2); border: 1px solid rgba(168,85,247,0.4); display: flex; align-items: center; justify-content: center; flex-shrink: 0; font-size: 0.75rem; color: #c084fc; font-weight: 700;">1</div>
      Set up the platform (Docker - we'll share the script)
    </div>
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: rgba(168,85,247,0.2); border: 1px solid rgba(168,85,247,0.4); display: flex; align-items: center; justify-content: center; flex-shrink: 0; font-size: 0.75rem; color: #c084fc; font-weight: 700;">2</div>
      Configure the agent and its connections
    </div>
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: rgba(168,85,247,0.2); border: 1px solid rgba(168,85,247,0.4); display: flex; align-items: center; justify-content: center; flex-shrink: 0; font-size: 0.75rem; color: #c084fc; font-weight: 700;">3</div>
      Write the instructions
    </div>
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: rgba(168,85,247,0.2); border: 1px solid rgba(168,85,247,0.4); display: flex; align-items: center; justify-content: center; flex-shrink: 0; font-size: 0.75rem; color: #c084fc; font-weight: 700;">4</div>
      Test and verify
    </div>
  </div>
  <div style="background: rgba(251,191,36,0.08); border: 1px solid rgba(251,191,36,0.3); border-radius: 12px; padding: 0.85rem 1.5rem; font-size: 0.85rem; color: #fbbf24; max-width: 420px;">
    💡 Not a techie? Just ask Claude to configure your OpenClaw - describe what you want and it'll set it up for you. Faster than doing it yourself.
  </div>
</div>

<!--
Start the OpenClaw setup now. While it's running, we'll keep talking. This wait is intentional - it's part of the lesson.
-->

---
layout: default
---

# While OpenClaw Builds - Going Deeper

<div class="grid grid-cols-2 gap-5 mt-6">
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #60a5fa; margin-bottom: 1rem;">What a good instruction looks like</div>
    <div style="font-size: 0.85rem; color: #d1d5db; line-height: 1.9; font-family: monospace;">
      <span style="color: #34d399;">✓</span> "If the message describes immediate property damage, fire, flood, or health risk - send an SMS alert to the owner."<br/><br/>
      <span style="color: #f87171;">✗</span> "Alert me if someone says URGENT."
    </div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #a855f7; margin-bottom: 1rem;">What the agent can output</div>
    <div style="font-size: 0.85rem; color: #9ca3af; line-height: 2; font-family: monospace;">
      <span style="color: #fbbf24;">Urgency:</span> <span style="color: #f87171; font-weight: 700;">9 / 10</span><br/>
      <span style="color: #fbbf24;">Reason:</span> <span style="color: #e5e7eb;">Immediate property damage</span><br/>
      <span style="color: #fbbf24;">Action:</span> <span style="color: #fb923c;">Alert sent to owner</span>
    </div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #ec4899; margin-bottom: 1rem;">Think about your own business</div>
    <div style="font-size: 0.9rem; color: #d1d5db; line-height: 1.8;">
      What is one thing that happens daily that you <strong style="color: white;">check manually</strong>?<br/><br/>
      Could a rule be written for it?
    </div>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.07); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #34d399; margin-bottom: 1rem;">What agents are not</div>
    <div style="font-size: 0.85rem; color: #d1d5db; line-height: 1.8;">
      <span style="color: #f87171;">✗</span> They do not know things you did not tell them<br/>
      <span style="color: #f87171;">✗</span> They are not perfect - always test<br/>
      <span style="color: #34d399;">✓</span> They are consistent - no bad days
    </div>
  </div>
</div>

---
layout: default
---

# Test and Break Your Agent

<div style="display: flex; flex-direction: column; gap: 1rem; max-width: 650px; margin: 1.5rem auto 0;">
  <div style="background: rgba(251,146,60,0.07); border: 1px solid rgba(251,146,60,0.25); border-radius: 16px; padding: 1.25rem 1.5rem;">
    <div class="flex items-center gap-2 mb-2">
      <carbon-warning-alt class="w-4 h-4" style="color: #fb923c;" />
      <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #fb923c;">Ambiguous - what does it do?</div>
    </div>
    <div style="color: #e5e7eb; font-style: italic; margin-bottom: 0.75rem;">"Water is leaking a little under my kitchen sink. Can someone come next week?"</div>
    <div style="font-size: 0.85rem; color: #9ca3af;">→ Leak mentioned, but they say "next week." Emergency or not?</div>
  </div>
  <div style="background: rgba(251,146,60,0.07); border: 1px solid rgba(251,146,60,0.25); border-radius: 16px; padding: 1.25rem 1.5rem;">
    <div class="flex items-center gap-2 mb-2">
      <carbon-warning-alt class="w-4 h-4" style="color: #fb923c;" />
      <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #fb923c;">Misleading keyword</div>
    </div>
    <div style="color: #e5e7eb; font-style: italic; margin-bottom: 0.75rem;">"URGENT!!! Can you send me your price list tonight?"</div>
    <div style="font-size: 0.85rem; color: #9ca3af;">→ "URGENT" in caps - but it's just a pricing request</div>
  </div>
</div>
<div style="margin-top: 1.5rem; background: rgba(168,85,247,0.08); border: 1px solid rgba(168,85,247,0.3); border-radius: 14px; padding: 1.25rem 1.5rem; text-align: center; max-width: 650px; margin-left: auto; margin-right: auto;">
  <div style="color: #c084fc; font-weight: 600; margin-bottom: 0.25rem;">Before you trust an agent - try to break it.</div>
  <div style="color: #9ca3af; font-size: 0.85rem;">Edge cases. Misleading wording. That's how you build confidence.</div>
</div>

---
layout: default
---

# OpenClaw - What We Just Saw

<div class="grid grid-cols-2 gap-6 mt-6 items-start">
  <div>
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #34d399; margin-bottom: 1rem;">What it can do</div>
    <ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.7rem;">
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        Fully open source - you own everything
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        Self-hosted - your data stays with you
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        No monthly fee for the platform itself
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #34d399;" />
        Unlimited customization
      </li>
    </ul>
  </div>
  <div>
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #f87171; margin-bottom: 1rem;">What it requires</div>
    <ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.7rem;">
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        Server setup and maintenance
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        Docker / technical knowledge to install
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        Time to learn the configuration
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-warning-alt class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #f87171;" />
        ~30 minutes just to get started
      </li>
    </ul>
  </div>
</div>
<div style="margin-top: 2rem; background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.1); border-radius: 14px; padding: 1.25rem 1.5rem; text-align: center;">
  <div style="color: #d1d5db; font-size: 0.95rem; line-height: 1.7;">
    OpenClaw is the right tool if you have a developer, or if you enjoy the technical side.<br/>
    <span style="color: rgba(255,255,255,0.4); font-size: 0.85rem; margin-top: 0.5rem; display: block;">We'll share the Docker install script so you can explore it after today.</span>
  </div>
</div>


---
layout: section
---

<div class="text-center">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1rem;">Part 4 · cont.</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; background: linear-gradient(to right, #60a5fa, #a855f7, #ec4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; line-height: 1.1;">The Same Agent<br/>in Setod</h1>
</div>

---
layout: default
---

# What is Setod?

<div class="grid grid-cols-2 gap-8 mt-6 items-start">
  <div>
    <p style="color: #d1d5db; font-size: 1rem; line-height: 1.8; margin-bottom: 1.25rem;">
      Setod is an agent platform built for business owners - not developers. Specially built for this workshop.
    </p>
    <ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.85rem;">
      <li class="flex items-center gap-3" style="color: #d1d5db;">
        <carbon-document class="w-5 h-5 flex-shrink-0" style="color: #60a5fa;" />
        Describe your agent in plain English
      </li>
      <li class="flex items-center gap-3" style="color: #d1d5db;">
        <carbon-plug class="w-5 h-5 flex-shrink-0" style="color: #a855f7;" />
        Connect your channels with a few clicks
      </li>
      <li class="flex items-center gap-3" style="color: #d1d5db;">
        <carbon-time class="w-5 h-5 flex-shrink-0" style="color: #ec4899;" />
        Schedule it to run - or trigger on messages
      </li>
      <li class="flex items-center gap-3" style="color: #d1d5db;">
        <carbon-machine-learning class="w-5 h-5 flex-shrink-0" style="color: #34d399;" />
        A built-in AI copilot helps you write better instructions
      </li>
    </ul>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 18px; padding: 1.75rem; font-family: monospace; font-size: 0.9rem;">
    <div style="font-size: 0.65rem; text-transform: uppercase; letter-spacing: 0.15em; color: #60a5fa; margin-bottom: 1rem;">You type this:</div>
    <div style="color: #e5e7eb; font-style: italic; margin-bottom: 1.5rem; line-height: 1.7;">"Watch my Telegram inbox. If a customer describes an emergency - flooding, fire, electrical hazard - send me an SMS alert right away."</div>
    <div style="font-size: 0.65rem; text-transform: uppercase; letter-spacing: 0.15em; color: #34d399; margin-bottom: 0.5rem;">Setod does the rest →</div>
    <div style="color: #9ca3af; font-size: 0.8rem; line-height: 1.8;">
      Agent created · Channel connected<br/>
      Instructions written · Ready to run
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

<div class="flex flex-col items-center justify-center h-full">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1.5rem;">Live Demo - Setod</div>
  <h2 style="font-size: 2.5rem; font-weight: 800; color: white; margin-bottom: 0.5rem;">Same Agent. 5 Minutes.</h2>
  <p style="color: #9ca3af; font-size: 1rem; max-width: 480px; line-height: 1.7; margin-bottom: 2.5rem;">We'll build the exact same emergency agent - and use the AI copilot to help write the instructions.</p>
  <div style="display: flex; flex-direction: column; gap: 1rem; max-width: 420px; width: 100%; text-align: left; margin-bottom: 2.5rem;">
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: linear-gradient(135deg, #2563eb, #7c3aed); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-chat-bot class="w-4 h-4 text-white" />
      </div>
      Create the agent - name and description
    </div>
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: linear-gradient(135deg, #2563eb, #7c3aed); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-plug class="w-4 h-4 text-white" />
      </div>
      Connect Telegram and SMS
    </div>
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: linear-gradient(135deg, #2563eb, #7c3aed); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-machine-learning class="w-4 h-4 text-white" />
      </div>
      Ask the copilot to write the instructions
    </div>
    <div class="flex items-center gap-3" style="font-size: 0.9rem; color: #d1d5db;">
      <div style="width: 28px; height: 28px; border-radius: 50%; background: linear-gradient(135deg, #2563eb, #7c3aed); display: flex; align-items: center; justify-content: center; flex-shrink: 0;">
        <carbon-chemistry class="w-4 h-4 text-white" />
      </div>
      Test with the same messages as before
    </div>
  </div>
</div>

---
layout: section
---

<div class="text-center">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1rem;">Agent 2</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; background: linear-gradient(to right, #60a5fa, #a855f7, #ec4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; line-height: 1.1;">Lead Finder Agent</h1>
  <carbon-portfolio class="w-12 h-12 mx-auto mt-4" style="color: rgba(96,165,250,0.6);" />
</div>

---
layout: default
---

# The Business Problem

<div style="margin-top: 1rem; border-left: 3px solid; border-image: linear-gradient(to bottom, #60a5fa, #a855f7) 1; padding: 1.5rem 2rem; background: rgba(59,130,246,0.05); border-radius: 0 16px 16px 0; max-width: 680px; margin-left: auto; margin-right: auto;">
  <p style="color: #e5e7eb; font-size: 1.05rem; line-height: 1.8; font-style: italic;">
    "I am a website designer in several business groups. Hundreds of messages are posted every day - I <strong style="color: #60a5fa; font-style: normal;">cannot read all of them.</strong>"
  </p>
</div>
<div class="grid grid-cols-2 gap-4 mt-5" style="max-width: 680px; margin: 1.25rem auto 0;">
  <div style="background: rgba(59,130,246,0.07); border: 1px solid rgba(59,130,246,0.25); border-radius: 14px; padding: 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <carbon-view class="w-4 h-4" style="color: #60a5fa;" />
      <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #60a5fa;">Obvious Lead</div>
    </div>
    <div style="color: #d1d5db; font-size: 0.9rem; font-style: italic;">"Does anyone know a good website designer?"</div>
  </div>
  <div style="background: rgba(168,85,247,0.07); border: 1px solid rgba(168,85,247,0.25); border-radius: 14px; padding: 1.25rem;">
    <div class="flex items-center gap-2 mb-2">
      <carbon-machine-learning class="w-4 h-4" style="color: #a855f7;" />
      <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #a855f7;">Hidden Lead</div>
    </div>
    <div style="color: #d1d5db; font-size: 0.9rem; font-style: italic;">"I just started a business and I'm trying to figure out how to sell online."</div>
  </div>
</div>
<div style="margin-top: 1.25rem; text-align: center; color: #9ca3af; font-size: 0.95rem;">
  Main question: <span style="color: white; font-weight: 600;">Can AI identify opportunities based on meaning, not keywords?</span>
</div>

---
layout: center
class: text-center
---

<div class="flex flex-col items-center justify-center h-full">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1.5rem;">Live Build - Setod</div>
  <h2 style="font-size: 2.5rem; font-weight: 800; color: white; margin-bottom: 0.5rem;">Build It Together</h2>
  <p style="color: #9ca3af; font-size: 1rem; margin-bottom: 2.5rem;">You know the pattern now. This one goes faster.</p>
  <div class="grid grid-cols-2 gap-4" style="max-width: 520px; width: 100%; text-align: left; margin-bottom: 2rem;">
    <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1rem 1.25rem;">
      <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: rgba(255,255,255,0.35); margin-bottom: 0.5rem;">The Business</div>
      <ul style="list-style: none; padding: 0; font-size: 0.85rem; color: #d1d5db; display: flex; flex-direction: column; gap: 0.3rem;">
        <li class="flex items-center gap-2"><carbon-code class="w-3 h-3" style="color: #60a5fa;" /> Website design</li>
        <li class="flex items-center gap-2"><carbon-shopping-cart class="w-3 h-3" style="color: #60a5fa;" /> E-commerce</li>
        <li class="flex items-center gap-2"><carbon-search class="w-3 h-3" style="color: #60a5fa;" /> SEO</li>
        <li class="flex items-center gap-2"><carbon-calendar class="w-3 h-3" style="color: #60a5fa;" /> Online booking</li>
      </ul>
    </div>
    <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1rem 1.25rem;">
      <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.1em; color: rgba(255,255,255,0.35); margin-bottom: 0.5rem;">Agent's Job</div>
      <ul style="list-style: none; padding: 0; font-size: 0.85rem; color: #d1d5db; display: flex; flex-direction: column; gap: 0.3rem;">
        <li class="flex items-center gap-2"><carbon-chat class="w-3 h-3" style="color: #a855f7;" /> Monitor groups</li>
        <li class="flex items-center gap-2"><carbon-decision-tree class="w-3 h-3" style="color: #a855f7;" /> Score leads</li>
        <li class="flex items-center gap-2"><carbon-notification class="w-3 h-3" style="color: #a855f7;" /> Notify on matches</li>
      </ul>
    </div>
  </div>
</div>

---
layout: section
---

<div class="text-center">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.3); margin-bottom: 1rem;">Wrap Up</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; background: linear-gradient(to right, #60a5fa, #a855f7, #ec4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text; line-height: 1.1;">Your Turn</h1>
</div>

---
layout: center
class: text-center
---

<div class="flex flex-col items-center justify-center h-full">
  <h2 style="font-size: 2.25rem; font-weight: 800; color: white; max-width: 560px; line-height: 1.3; margin-bottom: 2.5rem;">
    If you could build <span style="background: linear-gradient(to right, #60a5fa, #a855f7, #ec4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">one agent</span> for your business this week -<br/>
    what problem would it solve?
  </h2>
  <div class="grid grid-cols-3 gap-4" style="max-width: 680px; width: 100%; text-align: left;">
    <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.25rem; text-align: center;">
      <carbon-alarm class="w-8 h-8 mx-auto mb-2" style="color: #f87171;" />
      <div style="font-size: 0.85rem; color: #9ca3af;">Something you check manually every day</div>
    </div>
    <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.25rem; text-align: center;">
      <carbon-portfolio class="w-8 h-8 mx-auto mb-2" style="color: #60a5fa;" />
      <div style="font-size: 0.85rem; color: #9ca3af;">An opportunity you might be missing</div>
    </div>
    <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 14px; padding: 1.25rem; text-align: center;">
      <carbon-time class="w-8 h-8 mx-auto mb-2" style="color: #a855f7;" />
      <div style="font-size: 0.85rem; color: #9ca3af;">A task that always waits for you</div>
    </div>
  </div>
</div>

---
layout: default
---

# What To Take Home

<div class="grid grid-cols-2 gap-5 mt-6">
  <div style="background: rgba(168,85,247,0.07); border: 1px solid rgba(168,85,247,0.25); border-radius: 16px; padding: 1.5rem;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #c084fc; margin-bottom: 1rem;">If you want to explore OpenClaw</div>
    <ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.6rem;">
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-document class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #c084fc;" />
        Docker install script - shared in the group after today
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-link class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #c084fc;" />
        Best for: you have a developer, or you enjoy the technical side
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-time class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #c084fc;" />
        Budget a weekend to get comfortable
      </li>
    </ul>
  </div>
  <div style="background: rgba(99,102,241,0.08); border: 1px solid rgba(168,85,247,0.4); border-radius: 16px; padding: 1.5rem; box-shadow: 0 0 30px rgba(168,85,247,0.08);">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #60a5fa; margin-bottom: 1rem;">If you want to start today</div>
    <ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 0.6rem;">
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-rocket class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #60a5fa;" />
        Setod - link shared in the group after today
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-checkmark class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #60a5fa;" />
        No installation, no technical setup
      </li>
      <li class="flex items-start gap-2" style="color: #d1d5db; font-size: 0.9rem;">
        <carbon-machine-learning class="w-4 h-4 flex-shrink-0 mt-0.5" style="color: #60a5fa;" />
        The copilot helps you build from day one
      </li>
    </ul>
  </div>
  <div style="background: rgba(255,255,255,0.03); border: 1px solid rgba(255,255,255,0.08); border-radius: 16px; padding: 1.5rem; grid-column: span 2;">
    <div style="font-size: 0.65rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.15em; color: #34d399; margin-bottom: 0.75rem;">One honest reminder</div>
    <div style="color: #d1d5db; font-size: 0.9rem; line-height: 1.8;">
      The best way to learn agents is to build one for a problem you <strong style="color: white;">actually have.</strong> Start small. Test it. Break it. Improve the instructions. That's the whole loop.
    </div>
  </div>
</div>

---
layout: center
class: text-center
---

<div class="flex flex-col items-center justify-center h-full">
  <div style="font-size: 0.75rem; font-family: monospace; text-transform: uppercase; letter-spacing: 0.2em; color: rgba(255,255,255,0.25); margin-bottom: 2rem;">Thank you</div>
  <h1 style="font-size: 3.5rem; font-weight: 800; margin-bottom: 1rem; background: linear-gradient(to right, #60a5fa, #a855f7, #ec4899); -webkit-background-clip: text; -webkit-text-fill-color: transparent; background-clip: text;">
    Build something real<br/>this week.
  </h1>
  <p style="color: #6b7280; font-size: 1.1rem; max-width: 480px; line-height: 1.7; margin-bottom: 2.5rem;">
    You now understand what agents are, how they work, and what tools exist. The rest is practice.
  </p>
  <div style="font-size: 0.75rem; font-family: monospace; color: rgba(255,255,255,0.2); letter-spacing: 0.1em;">
    Observe · Understand · Decide · Act
  </div>
</div>
