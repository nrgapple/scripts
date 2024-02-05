# ChatGPT command generator cli

## Installation

Put the `ai_command_generator` folder somewhere.

Copy the `.env.sample` file to `.env` and fill in the value for your OpenAI API key.

Add the `ai_command_generator` folder to your `PATH` environment variable. You can do that by adding the following line to your `.bashrc` or `.zshrc` file:

```bash
export PATH=$PATH:/path/to/ai_command_generator
```

Replace `/path/to/ai_command_generator` with the actual path to the `ai_command_generator` folder.

Make sure to reload your shell or run `source ~/.bashrc` or `source ~/.zshrc` to apply the changes.

Last make the script executable by running `chmod +x /path/to/ai_command_generator/ai_command_generator`. Replace `/path/to/ai_command_generator/ai_command_generator` with the actual path to the `ai_command_generator/ai_command_generator` script.

### Bonus: Add an alias

You can add an alias to your `.bashrc` or `.zshrc` file to make the command easier to use. Add the following line:

```bash
alias aicmd='ai_command_generator'
```

Now you can use the `aicmd` command to generate commands.

## Usage

Run the `ai_command_generator` command to generate a command. You can pass a prompt as an argument to the command. For example:

```bash
> aicmd "find all files in the ~/BuiltSource folder and down with the word BUILT_API in it"
find ~/BuiltSource -type f -name "*BUILT_API*"
```
