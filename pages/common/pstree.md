# pstree

> This commands shows all the processes running currently along with associated child process, in a tree like format similar to ‘tree‘ command output.

- The basic syntax of pstree is:

`pstree [options][pid or username]`

- To use it more convinently:

`pstree | less`

- As is the case with most command line programs, pstree has several options that greatly enhance its flexibility and usefulness. One of the most commonly used is -p, which tells it to show process identification numbers (PIDs):

`pstree -p`

- The -n option instructs pstree to sort its output in the order of the PIDs instead of in the default alphabetic order:

`pstree -np`

- The -h option highlights (or shows in bold) the current process and all of its ancestors, if highlighting is permitted by the particular system:
 
`pstree -h`

- The -u option tells pstree to show the owner of a process (i.e., the user that started it) in parenthesis whenever its ownership differs from that of its parent:

`pstree -u`

- The -l option prevents the truncation of long lines of output that can occur when the display screen is not sufficiently wide. It does this by wrapping (i.e., carrying over) any excess output to the next line:

`pstree -l`

- The -a option shows the command line arguments for each process that was initiated by a user (instead of by another process) by issuing a command with arguments:

`pstree -a`
