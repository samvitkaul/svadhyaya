# Visualizing and maintaining Svādhyāya

This repo is a Git-native mathematical notebook. **Obsidian is a viewer/editor, not the source of truth.** The files are ordinary Markdown with LaTeX mathematics and relative links that work on GitHub too.

## Quick start: Obsidian

1. Install [Git](https://git-scm.com/) and [Obsidian](https://obsidian.md/).
2. Clone the existing repository, from a terminal:

   ```bash
   git clone https://github.com/samvitkaul/svadhyaya.git
   ```

3. Open Obsidian. Choose **Open folder as vault** and select the cloned `svadhyaya/` directory. Do not make a fresh empty vault.
4. Start with [the connections map](../maps/connections.md) and [the algebra map](../maps/algebra.md).
5. Use **Command palette** (`Ctrl/Cmd+P`) and run **Open graph view** to show note connections. The **Local graph** command shows neighbors of one note; its depth can be adjusted in graph settings. Use the **Backlinks** pane to discover inbound links.
6. Search for an idea such as `splitting`, `kernel`, `group action`, or `convolution`. Read both the formal concept and its exploratory context.

**Links:** This repository intentionally uses `[Modules](../concepts/modules.md)`, not Obsidian-only `[[wikilinks]]`, so it is readable on GitHub. Relative Markdown links are understood by Obsidian. An isolated note will not appear well connected until there are real internal links. Obsidian's graph visualizes note-level links; it does **not** independently discover semantic similarities.

**Math:** `$...$` and `$$...$$` are used for inline/display LaTeX. Inspect source if a particular renderer misinterprets a construct.

## Obsidian views for different purposes

| View | Role |
|---|---|
| Global Graph | Survey the whole collection; filter by paths such as `explorations/` |
| Local Graph | Trace near neighbors of one theorem or question |
| Backlinks | See which later ideas depended on an earlier note |
| Canvas (core plugin) | Curated argument flow: conjecture → counterexample → correction |
| Search | Find precise terminology, LaTeX expressions, and unanswered questions |

Use **Canvas** for hand-authored maps rather than expecting the global graph's force layout to communicate mathematical logic.

## Editing and syncing

From a terminal in the cloned repository:

```bash
git pull --rebase
# Edit in Obsidian or VS Code
git status
git diff --check
git add .
git commit -m "Extend exploratory notes"
git push
```

Alternative: install the [Obsidian Git community plugin](https://community.obsidian.md/plugins/obsidian-git) through **Settings → Community plugins → Browse → Git**, then enable it. It can expose commit/pull/push actions inside Obsidian. The Git executable and remote authentication still need to be configured. **Keep auto-commit/auto-push off at first**; review corrections and avoid concurrent editors on two devices.

If Git reports a merge conflict, resolve the conflicting Markdown and inspect mathematics before committing. Git history preserves changes but should not replace explicit explanations of false starts in the text.

## Other tools

- **[VS Code](https://code.visualstudio.com/)**: edit/search Markdown, review diffs, and run Git commands. Good for working with Codex or scripting link checks.
- **GitHub**: browse the canonical files online and review pull requests and history. GitHub is not a semantic graph viewer.
- **Mermaid**: add small, explicit flowcharts inside Markdown, such as an extension classification argument. GitHub supports Mermaid diagrams.
- **[Quartz](https://quartz.jzhao.xyz/)**: optional future *public digital garden* with search, backlinks, and a graph. This requires a separate publishing setup; it is **not configured** here. Review content before publishing anything automatically.
- **Python / NetworkX**: optional graph analyses (clusters, disconnected notes, degree). Parse only repository-internal Markdown links; treat these as editorial signals, not mathematical proof.

## A useful working habit

Read an exploration chronologically, including its errors. Then follow its **Correction**, **Consolidation**, and **Connections** links. Use the local graph to compare the narrative path with the abstract concept map.

Every new note should express links using relationships: **motivates**, **example of**, **generalizes**, **contrasts with**, **depends on**, **corrected by**. Few justified links are better than an indiscriminate cloud.

## Privacy

As of initial setup, the repository is public. Do not commit unreviewed ChatGPT exports, private chat URLs, confidential design details, passwords, or employer-specific architecture. Keep raw source conversations outside the public repo. The exploration reconstructions included here are **based on available conversation history and summaries, not verified verbatim transcripts**; any direct quote should be checked against its original source before publication.
