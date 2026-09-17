# Using VS Code for This Course

You don't need VS Code for any of these labs — every file-creation step works fine typed directly into a
terminal. But if you have VS Code installed, it's a noticeably nicer way to work through this course: syntax
highlighting catches YAML indentation mistakes before you even run anything, and you get a built-in terminal so
you never have to alt-tab between an editor and a command line.

## One-time setup

1. **Open the course folder in VS Code.** From a terminal, `cd` into wherever you cloned/unzipped this course, then run:
   ```bash
   code .
   ```
   (If `code` isn't recognized: open VS Code, press `Ctrl+Shift+P` / `Cmd+Shift+P`, run "Shell Command: Install
   'code' command in PATH", then try again.)

2. **Install these extensions** (Extensions panel, `Ctrl+Shift+X` / `Cmd+Shift+X`) — all optional, but each pays
   for itself quickly in this course:
   - **YAML** (`redhat.vscode-yaml`) — catches indentation errors as you type, which matters a lot from Module 4 onward
   - **Docker** (`ms-azuretools.vscode-docker`) — lets you right-click a Dockerfile to build it, and browse images/containers in a sidebar
   - **Kubernetes** (`ms-kubernetes-tools.vscode-kubernetes-tools`) — cluster/resource browser, useful from Module 4 onward
   - **Docker Compose** support is bundled into the Docker extension above

## The pattern used throughout this course

Wherever a lab has you create a file with a command like:

```bash
cat > compose.yaml <<'EOF'
services:
  web:
    image: nginx
EOF
```

That single command does two things: it creates the file, and it writes the given content into it — convenient
for a terminal-only workflow, but not how you'd naturally work in an editor. Any lab that includes one of these
will also show a **"Using VS Code instead"** box directly underneath it, telling you exactly what file to create
and what to paste into it. Use whichever approach you prefer — they produce identical results.

## Everyday workflow

- **Creating a file:** Right-click a folder in the Explorer panel (left sidebar) → **New File**, type the
  filename (matching exactly what the lab specifies, including the extension), then paste the content shown in
  the lab and save with `Ctrl+S` / `Cmd+S`.
- **Running commands:** Open the integrated terminal with **Terminal → New Terminal** or `` Ctrl+` `` /
  `` Cmd+` ``. This opens a real shell already pointed at your project folder — every `docker`, `docker compose`,
  `kubectl`, and `helm` command in this course runs here exactly as written; VS Code doesn't change any command
  syntax, only how you get files onto disk.
- **Editing an existing file:** Click it in the Explorer panel to open it, edit directly, and save. No need to
  retype a whole file with a new heredoc just to change one line.
- **Multiple terminals:** Each lab tends to use one terminal, but feel free to open a second one (the `+` icon in
  the terminal panel) if a lab has you run something in the background (like `docker compose up`, without `-d`)
  while running other commands in parallel.

## What VS Code does NOT change

VS Code doesn't run Docker or Kubernetes itself — Docker Desktop (or Docker Engine) and `kind`/`kubectl` still do
all the real work, exactly as if you'd typed everything by hand in a plain terminal. VS Code is purely a more
convenient way to create/edit files and run those same commands — nothing in this course behaves differently
because you're using it.
