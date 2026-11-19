# scaled-thinking modules

Free tools for your AI. Each module helps your AI with one job: it does the work with you, and you
get better at it. Every module is free and runs on the AI you already have; a line below says when
one needs more. What you share goes only to the AI and services you choose. scaled-thinking has no
server, so it never sees it.

To start, ask your AI to read this list and suggest a module for you, or pick one under Ready to use
and open its link.

## Ready to use

An agent is an AI assistant that does work, not just chat: it opens your files, runs programs and
checks the result. An agent app is the program you run your agent in, on your computer or in the
browser.

- **[present-together](https://github.com/scaled-thinking/present-together):** Give better talks: an
  AI coaches you and builds the interactive parts.
  Any agent app that can open files and run programs builds and tests the activities; coaching alone
  works in almost any AI chat. Hosting a live activity is optional and can cost money; the agent
  shows the cost and asks first.
- **[open-research-loops](https://github.com/scaled-thinking/open-research-loops):** Test your
  research idea with AI and see what really holds up.
  Any agent app that can read files, run commands and search the web, plus uv and Python 3.12 or
  newer on Windows or Linux. The offline example runs in a terminal and calls no model.

## In progress, not public yet

These modules exist and are being tested. They are not public yet, so you cannot install them yet.

- **shape-together:** Sharpen a rough idea: see its assumptions and a first test.
- **spec-together:** Turn your idea into a clear plan that can be built and tested.
- **build-together:** Get a first working version of your idea, tested and explained.
- **challenge-together:** Get an honest second opinion on your plan before you start.
- **distill-together:** Turn sources into short notes you can trust, with exact quotes.
- **learn-together:** Practise with your own cards and see a week later what stayed.
- **plug-together:** Connect modules to your AI in one place; each stays off until you switch it on.
- **account-together:** See what your AI used and did, kept on your computer.
- **start-together:** Start your own module, with the family's checks built in.

Questions and feedback: contact@scaled-thinking.com

## Details

### [present-together](https://github.com/scaled-thinking/present-together)

- What it does: It coaches you on your message and on activities that let your audience take part,
  such as a phone poll where everyone commits to an answer first. The agent then builds, tests and,
  if you want, hosts the interactive parts, and you keep a method card for your next talk. You
  decide the message, the activity and your verdict on the first version of the activity.
- Who it suits: Teachers and students preparing a talk, lecture or seminar that is not graded or
  submitted.
- Interfaces:
  - Skill: `skills/interactive-classroom-presentation/SKILL.md`, with `AGENTS.md` as the entry for
    agents.
- Install:
  - Claude Code: copy `skills/interactive-classroom-presentation` into `.claude/skills/` in your
    project folder, or paste the starter prompt from the README.
  - Codex: copy `skills/interactive-classroom-presentation` into `.agents/skills/` in your project
    folder, or paste the starter prompt from the README.
  - Other apps: paste the starter prompt from the README; the agent reads `AGENTS.md` and the skill
    from the repository.
- Licence: Apache-2.0 for code, `SKILL.md` and prompt files; CC BY 4.0 for texts, teaching material
  and images. Every commit before the licence change, including version 1.0.0, stays under MIT, and
  third-party material keeps its own terms (see NOTICE).

### [open-research-loops](https://github.com/scaled-thinking/open-research-loops)

- What it does: You set a research question and what would disprove it before any result exists. The
  agent writes the code and runs several attempts in parallel, a protected scoring program that the
  attempts cannot touch scores each one the same way, and you give the verdict. You get a report
  that tags each result as measured or simulated and keeps negative results; in coached mode you
  also get a research brief and your own method card.
- Who it suits: Researchers and students who want to test an idea with AI and keep honest evidence,
  without coding themselves.
- Interfaces:
  - Skill: eight skills under `skills/`, with `skills/rloop-coach/SKILL.md` for coached mode and
    `AGENTS.md` as the entry for agents.
  - CLI: `rloop`, for example `rloop init`, `rloop status`, `rloop report` and `rloop pilot`.
  - MCP: the six tools each parallel attempt may use, `read_contract`, `read_findings`,
    `read_artifact`, `register_variant`, `write_artifact` and `submit_result`, and nothing else
    (`docs/DESIGN.md`).
  - Python: `research_loops`, distributed as `research-loops` from source.
- Install:
  - Claude Code: paste a starter from the README; the agent clones the repository, runs
    `uv sync --locked` and follows `AGENTS.md`.
  - Codex: paste a starter from the README; the agent clones the repository, runs `uv sync --locked`
    and follows `AGENTS.md`.
  - Other apps: paste a starter from the README into any app that can clone a repository, run
    commands and read `AGENTS.md`.
- Licence: Apache-2.0 for code, `SKILL.md` and prompt files; CC BY 4.0 for texts and images. The
  adapted review rubric and the skill versions published before the licence change keep CC BY 4.0
  (see NOTICE).
