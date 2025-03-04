> A paradigm is a distinct set of concepts, thought patterns, theories, or methodologies that forms a framework through which we understand and interpret reality. It represents a fundamental model or pattern that shapes how we perceive, think about, and approach problems within a particular domain.

# Paradigm Shift (`pash`)

`pash` is a command line tool for running LLM prompts from files against files with goal to modify files.


## Running `pash`

`pash prompt_file_path` where `prompt_file_path` is a path to a prompt file. Prompt file may contain text, markdown, markdown with metadata block. `pash` produces extensive logs, requiring user interaction on every step of its run.

## Pash prompt file

First prompt in the assistant conversation resides in a file. Optionally there is also a markdown metadata which contains info from previous prompt files runs: assistant id, thread id, run id, etc. These values are updates on each tool run multiple times the tool goes through various steps (thread creation, sending files into the thread, etc).
