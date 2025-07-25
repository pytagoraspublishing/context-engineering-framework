# Generate Template PRP

## technology-name: $ARGUMENTS

1. Create a new branch called @ARGUMENTS, if @ARGUMENTS is not a valid branch name, then find a  suitable branch name.
2. Switch to this branch
3. Create the folder @use-cases/{technology-name} and then create the file @PRPs/INITIAL-{technology-name}.md and copy the content of @PRPs/INITIAL.md into it.

Prompt the user to fill in the @PRPs/INITIAL-{technology-name}.md file. This is a notification not a todo. Give the user the options 1. to let the AI fill in the INITIAL-{technology-name}.md 2. to run the command `/generate-template-prp @PRPs/INITIAL-{technology-name}.md` 3. to abort the process.
    1. If the user selects the option to let the AI fill in the INITIAL-{technology-name}.md, then let the AI fill in the INITIAL-{technology-name}.md and then ask the user to run the command `/generate-template-prp @PRPs/INITIAL-{technology-name}.md`.
    2. If the user selects the option to run the command `/generate-template-prp @PRPs/INITIAL-{technology-name}.md`, then run the command. 
    3. If the user selects the option to abort the process, then abort the process and clean up the folder @use-cases/{technology-name}/ and switch back to the main branch and delete the branch @ARGUMENTS.
