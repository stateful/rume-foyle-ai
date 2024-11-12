---
runme:
  id: 01J1TBMRJ7VHHB0F9N2SDBKEQE
  version: v3
---

### Runme Notebook's Hello-World

Run some commands in a Notebook! First click the 'allow' button to login to VS Code with your user.

### Step one:

You should see a `▶️ play` button to the left of the command (on hover), just click it! Now you should see terminal output, click the `[Save]` button below the command to securely store its output and metadata (sign in if you haven’t). Then click `[Open]`, to go check it out in the browser.

```sh {"id":"01J1TBTVH2HPJNW6SXTTW70RMS","name":"step1-echo-command"}
$ echo "hello-world"
```

### Step two:

When you `▶️ play` this command, you should see an input prompt pop-up, this is the notebook utilizing the VS Code built in UI for prompts and then storing the value in an environment variable. You should see a `welcome message`, customized with your input in the terminal output. Click `[Save]` for this cell.

```sh {"id":"01J1TCBTA6K6BQ2K1P0FFFGDDF","name":"step2-input-command"}
$ export YOUR_NAME="New Runme User"
$ echo "Welcome to Runme Notebooks, ${YOUR_NAME}"
```

### What next!?

- Create a new command cell, by hovering over the area in the notebook you want, and click `+ Code`, write a command and `▶️ play` it.
- Check out everything Runme can do in the /examples directory
- Create a new Markdown file `exploring.md` with the file explorer and build a new Notebook workflow from scratch.
- Open the [Stateful Cloud](https://cloud.stateful.com) to see the commands you ran, configure your workspace, and start collaborating with your team.
- Check out wide range of cool stuff notebooks can do, [Runme docs](https://runme.dev)
