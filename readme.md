> A paradigm is a distinct set of concepts, thought patterns, theories, or methodologies that forms a framework through which we understand and interpret reality. It represents a fundamental model or pattern that shapes how we perceive, think about, and approach problems within a particular domain.

# Paradigm Shift (`pash`)

`pash` is a command line tool for running LLM prompts from files against files with goal to modify files.


## Running `pash`

Running without installation directly from the github:

```
npx github:podgorniy/pash PROMPT_FILE
```

Running after installation:

`pash prompt_file_path` where `prompt_file_path` is a path to a prompt file. Prompt file may contain text, markdown, markdown with metadata block. `pash` produces extensive logs, requiring user interaction on every step of its run.

## Pash prompt file

Main prompt for the assistant resides in the input file provided into the `pash` tool call. Optionally file may contain markdown metadata with data from previous prompt files runs: assistant id, thread id, run id, etc. This data is updated on each tool run multiple times. And this data is used by the tool. For example you may choose to reuse `threadId` from previous runs as you're iterating on your prompt. This will save you API costs. In order not to reuse assistant/thread just remove corresponding lines from the prompt file.
