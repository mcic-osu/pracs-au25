# PLNTPTH5006-AU25: Feedback on Graded Assignment 3 - Elisabeth Garner

- Author: Menuka Bhandari
- Date: 2025-08-10

You earned 7/10 points on this assignment. Well done!
- Overall feedback:
  - You have good understanding containers,and modules.

- Specific feedback:
  - It looks like you have confusion in assigning shell variables and script variables. 

## Part A - Setting up

- Your Markdown file: `/fs/ess/PAS2880/users/egarner99/GA3/README.md`

- Points awarded: 1.5/1.5

## Part B - Running two scripts

- Points awarded: 1/2

5. Part of this question was explain your results rather than just writing your results. I have provided the detailed explanation below:

    A. Third argument is not defined in the command.

    B. Although the script is called with 4 arguments, it only requires 3 arguments to run. Any additional arguments beyond these 3 are ignored. However, if you provide fewer arguments than the script expects, it will produce an error, as seen in example 5A ( $3: unbound variable)

    C. "Oct09 Oct10" is inside a quotation mark, so, it is considered as a single argument.

6. You were supposed to concatenate the files that you copied earlier in the question number 3. Instead, you provided the command to copy it from `garrigos-data/fastq/` directory and changed the metadata of garrigos-data/meta/metadata.tsv with concatenated file.

## Part C - A shell script that prints a specific line
- Points awarded: 2/3
7. The command you provided will not just print one line but prints five lines because your second argument asks to print 5 lines. If you had provided `bash scripts/printline.sh data/metadata.tsv 1` for the script `tail -n +2 "$1" | head -n "$2"`, you would have gotten one line. The easiest way to get just one line would have been to pipe the head command with the tail command as suggested in the hint.

8. Your script to print the just one line is not correct, but you have redirected output in a correct way.

9. You have correctly defined the shell variables  `meta="metadata.tsv"` and `number="9"` `bash scripts/printline.sh $meta $number > results/"$meta"_"$number".txt` is the right way of redirection.

## Part D: Containers
- Points awarded: 1/1

## Part E: Modules and Pandoc
- Points awarded: 1/1.5

## Part F: Publish your repo on Github
- Points awarded: 0.5/1

- You have pushed just the README file rather than whole repository of GA3.
- To add the whole repository, you should link your remote folder with the local folder and push it.
[link the local and remote repo](https://mcic-osu.github.io/pracs-au25/week04/w4b_github.html#remote-repositories)

