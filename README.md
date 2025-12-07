<p align="center">
  <img src="images/logo_transparent.png" alt="MarkTree logo" width="220" />
</p>

<h1 align="center">MarkTree</h1>

<p align="center">
  <strong>MarkTree is basically a Swiss Army Knife for AI Development</strong> — built for working with <em>any</em> agentic coding system.<br/>
  Copy clean, LLM-ready Markdown context from VS Code in seconds. It will save you countless hours.
</p>

<p align="center">
  <em>Directory trees • file contents • selections • tabs • symbols • Problems panel • Git diffs • token counting • chunking</em>
</p>

---

## What you get

MarkTree turns your workspace context into **paste-perfect Markdown**:

- **Right-click → Copy → Paste into your agent** (ChatGPT / Claude / Gemini / Copilot Chat / Cursor / Continue / etc.)
- **Readable, structured output** with paths + fenced code blocks
- **Local-first**: your code stays on your machine (see [Privacy](#privacy--security))

---

## See it in action

### Copy a Markdown directory tree

<img src="images/copy_md_tree.gif" alt="Copy Markdown tree demo" />

### Copy file contents as Markdown

<img src="images/copy_md_files.gif" alt="Copy Markdown files demo" />

### Copy a tree _and_ the files under it

<img src="images/copy_md_tree_and_files.gif" alt="Copy Markdown tree and files demo" />

### Live token counter (status bar)

<img src="images/token_counter.gif" alt="Token counter demo" />

---

## Why MarkTree (especially for AI / agentic workflows)

When you’re working with an AI assistant, the biggest time sink is always the same: **collecting and formatting context**.

MarkTree removes the glue work:

- **No more “copy file… paste… repeat…”**
- **No more hand-writing directory trees**
- **No more “what files am I missing?”**
- **No more guessing token limits**

You get fast, consistent context that agents can actually use.

---

## Quick start

1. Install **MarkTree** from the VS Code Marketplace.
2. In the Explorer, **right‑click** a folder or file:
   - **MarkTree → Copy Md Tree**
   - **MarkTree → Copy Md File(s)**
   - **MarkTree → Copy Md Tree & Files**
3. Paste into your agent/chat/issue/PR. Done.

---

## Commands (what’s included)

### Core “copy context” commands (Free)

- **Copy Md Tree** — copy a directory outline as Markdown
- **Copy Md File(s)** — copy one or many files as Markdown (with code fences)
- **Copy Md Tree & Files** — include the tree preview + the file contents
- **Copy Active File as Markdown**
- **Copy Selected as Markdown** (editor selection)
- **Copy as Markdown** (terminal selection)
- **Copy Problems for Active File**
- **Copy All Problems** (workspace Problems panel)
- **Copy Symbol as Markdown** (pick a function/class/etc.)
- **Copy all tabs as Md**
- **Copy tabs to the left as Md**
- **Copy tabs to the right as Md**
- **Add to MD Ignores** / **Remove from MD Ignores** (quickly tweak ignore list)

### AI utilities (Free)

- **Select Token Counter Model** — pick a model to count tokens accurately
- **Clear Model Cache** — refetch model metadata (used by the token counter)

### Pro features (requires a MarkTree Pro license)

- **(Pro) Copy Staged Git Changes as Markdown**
- **(Pro) Copy Selected Git Commits** (copies diffs for chosen commits)
- **(Pro) Generate Structure from Clipboard Tree** (scaffold folders/files from a Markdown tree)
- **(Pro) Chunk Editor by Model Size** (split big files/selections into model-friendly chunks)

---

## Output format (what you paste)

MarkTree generates Markdown like:

- Optional **tree preview** (in a fenced block)
- Then **one section per file**, with a path header and a fenced code block

This makes it easy for agents (and humans) to navigate context without losing file boundaries.

---

## Configuration

Open **Settings** and search for “MarkTree”, or add to your `settings.json`:

```json
{
  "marktree.gitignore": true,
  "marktree.ignoreBinary": true,
  "marktree.additionalIgnores": [".git", ".vscode/", "pnpm-lock.yaml"],
  "marktree.showCopyingMessage": false,
  "marktree.showCopiedMessage": true,
  "marktree.showTokenCounter": true
}
```

Notes:

- **`marktree.gitignore`**: respects your repo ignore rules (great for keeping prompts clean).
- **`marktree.ignoreBinary`**: skips binary contents (so you don’t paste gibberish).
- **`marktree.additionalIgnores`**: your “prompt hygiene” list (build outputs, lockfiles, generated folders, etc.).

---

## MarkTree Pro

MarkTree Pro is for people who live in agentic loops and want fewer interruptions:

- Paste **staged diffs** or **selected commit diffs** instantly
- Turn a **Markdown tree into a real scaffold** in seconds
- **Chunk large files** to fit model limits (with tokenizer + overlap controls)

To activate:

1. Run **“MarkTree: Enter License Key”**
2. Paste your key
3. Pro commands unlock automatically

---

## Privacy & Security

MarkTree is designed to be **local-first**:

- Workspace content (paths, files, tree, selections, diagnostics, Git output) is processed **on your machine**
- MarkTree **does not** collect analytics/telemetry
- Content is copied only to **your clipboard**

Network access happens only for:

- **Pro license validation** (your license key is sent to the licensing endpoint)
- **Model metadata fetch** for the token counter (fetched from OpenRouter model listings)

Read the full policy in **`PRIVACY_POLICY.md`**.

---

## Troubleshooting (common gotchas)

- **“Why didn’t it copy some files?”**
  Check `marktree.gitignore` and `marktree.additionalIgnores`.

- **“Binary file: content not displayed”**
  That’s intentional when `marktree.ignoreBinary` is enabled.

- **Token counter says “Models unavailable”**
  The model list fetch failed (network/offline). Try again later or run **Clear Model Cache**.

---

## Support

If MarkTree saves you time, consider upgrading to Pro or sharing it with your team. 🙂
