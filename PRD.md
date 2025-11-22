# opencode-queue

## Description

CLI tools to queue up prompts for opencode.

Interface:
```
opencode-queue <time> <prompt>

Example:
opencode-queue "1 hour" "What is the meaning of life?"
```

They should be launched according to the time they are scheduled to be run.

In the above example, the prompt will be queued for 1 hour from now.

Should also support specifying a specific time.

Should also support the ability to specify an existing session in opencode.

## Architecture

- Rust
- clap (CLI parser)
- invokes opencode via its server commands https://opencode.ai/docs/
