# MarkTree

MarkTree is a dev power tool for effortlessly copying any aspect of source control: directory structures, file contents, tabs, and even Git diffs, into Markdown. Take advantage of the latest LLMs or Agentic systems like V0, Gemini, GPT 4.1 or new Claude releases without waiting for GitHub Copilot or Cursor support. Provide advanced context beyond what these IDEs support.

[![Get MarkTree Pro](images/logo.png)](https://buymeacoffee.com/lkpuiu42en/e/395935)

# Pro

[**MarkTree Pro**](https://buymeacoffee.com/lkpuiu42en/e/395935) unlocks extra features for advanced users. If you’re constantly handling multiple commits, deeply reviewing diffs, or wanting the ultimate control in how you share your code with AI or collaborators, MarkTree Pro has you covered.

**Pro Feature Highlight:**

- **Generate Structure from Clipboard Tree**: Copy a Markdown‑style directory tree to your clipboard, right‑click any folder, and instantly scaffold the entire structure—folders and files—inside your workspace.
- **Copy Staged Git Changes**: Gather your staged Git changes into Markdown diffs—perfect for partial commits or quick reviews.
- **Copy Git Diffs for Selected Commits**: Use a QuickPick to select multiple commits, then MarkTree gathers the `git show` output for each commit and merges them into one Markdown snippet.
- **Chunk Editor by Model Size**: Choose a model (with its max message tokens from an up‑to‑date list), pick a sentence/code splitter, optionally add per‑chunk instructions, and MarkTree will split the active editor (or selection) into token‑budgeted chunks, each opened in its own editor tab. Prevents overrunning model limits while prepping prompts.
- **Priority License Validation**: Faster updates and priority support.
- And more coming soon!

**Coming Soon!**

- **Copy Symbol and References**: Copy a symbol and all of its references recursively into Markdown snippets.

Click the image or link above to get MarkTree Pro. Once purchased, you'll receive a license key to unlock all Pro features directly in your existing MarkTree installation.

---

# Free

- **Copy Md Tree**: Copies a directory’s tree structure as Markdown.
- **Copy Md Files**: Copies the contents of files as Markdown code blocks.
- **Copy Md Tree & Files**: Copies both the directory tree and file contents.
- **Copy Tabs**: Copies the contents of all currently open file-based tabs.
- **Copy Tabs to the Right**: Copies only the open file-based tabs to the right of the current active tab.
- **Copy Tabs to the Left**: Copies only the open file-based tabs to the left of the current active tab.
- **Copy Problems from Active File**: Copies all errors/warnings (diagnostics) for the currently active file, including relevant code snippets.
- **Copy Selected as Markdown**: Copies your current selection as a single Markdown code block.
- **Copy Symbol from Active File**: Lets you pick any symbol (class, function, etc.) and copy it as a Markdown code block.
- **Copy Terminal Selection**: Copy selected terminal text as a Markdown code block.
- **.gitignore Support**: Optionally respect your workspace’s `.gitignore` files and custom ignore entries.
- **Binary File Skipping**: Optionally skip binary files when copying directory contents.

---

### Copying Open Tabs as Markdown

If you frequently work with multiple files at once, MarkTree lets you copy the contents of all currently open file-based tabs as Markdown. You can also limit copying to tabs on the right or left of the active one. This makes it easy to share precisely the subset you need.

- **Copy All Tabs**: Copies all open file-based tabs.
- **Copy Tabs to the Right**: Copy a selection of files opened to the right of the current focus.
- **Copy Tabs to the Left**: Quickly capture the files opened to the left side.

### Copying Problems from the Active File

MarkTree can collect and copy all **diagnostics** (errors, warnings, etc.) for your currently active file—complete with **line numbers**, **messages**, and **code snippet** context.

When you run **Copy Problems from Active File**, you’ll get a Markdown snippet like:

---

#### Problems for /path/to/file.ts

##### Issue 1 of 2

- **Severity**: Error
- **Line**: 12, **Column**: 5
- **Source**: eslint
- **Message**: Unexpected token
- **Code**: 1234

```ts
// Lines 10-14:
10  const foo = {
11    bar: 42
12    baz: 99 // <-- Missing comma
13  };
14
```

---

## Copying Md Tree

```sh
/Users/falven/Source/turborepo/examples/basic/packages/lib
├── src
│   └── index.ts
├── package.json
└── tsconfig.json

2 directories, 3 files
```

![Copy Md Tree](images/copy_md_tree.gif)

---

## Copying Md Files

Each file is formatted as a code block with automatically detected language:

`src/index.ts`

```ts
export const multiply = (a: number, b: number) => {
  console.log('Breakpoint in multiply');
  return a + b;
};
```

`package.json`

```json
{
  "name": "@repo/lib",
  "version": "0.0.0",
  "type": "module",
  ...
}
```

`tsconfig.json`

```json
{
  "extends": "@repo/typescript-config/base.json",
  "compilerOptions": {
    "outDir": "dist",
    "sourceRoot": "../../packages/lib/src"
  },
  "include": ["src"],
  "exclude": ["node_modules", "dist"]
}
```

![Copy Md Files](images/copy_md_files.gif)

---

### Copying Md Tree & Files Together

```sh
/Users/falven/Source/turborepo/examples/basic/packages/lib
├── src
│   └── index.ts
├── package.json
└── tsconfig.json

2 directories, 3 files
```

`src/index.ts`

```ts
export const multiply = (a: number, b: number) => {
  console.log('Breakpoint in multiply');
  return a + b;
};
```

`package.json`

```json
{
  "name": "@repo/lib",
  "version": "0.0.0",
  ...
}
```

`tsconfig.json`

```json
{
  "extends": "@repo/typescript-config/base.json",
  "compilerOptions": {
    "outDir": "dist",
    "sourceRoot": "../../packages/lib/src"
  },
  "include": ["src"],
  "exclude": ["node_modules", "dist"]
}
```

![Copy Md Tree & Files](images/copy_md_tree_and_files.gif)

---

## Requirements

No special dependencies are required. Just install and start copying Markdown trees and files!

## Known Issues

No known issues at this time. Please report any problems or feature requests on our [GitHub repository](https://github.com/Falven/marktree-docs/issues).

---

Like the extension? Consider supporting it with a donation. Your support helps keep the project alive and allows me to dedicate more time to its development. Thank you!

<a href="https://www.buymeacoffee.com/lkpUiU42EN" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-violet.png" alt="Buy Me A Coffee" style="height: 40px !important;width: 150px !important;"></a>

**Enjoy using MarkTree! 🌳**

Looking for more power? Don’t forget to check out [**MarkTree Pro**](https://buymeacoffee.com/lkpuiu42en/e/395935) for advanced Git diffing and more!

## Privacy Policy

MarkTree does **not** transmit or store anything you copy.

See the full policy → [Privacy Policy](PRIVACY_POLICY.md).
