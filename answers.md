Answer 1: git version 2.17.1
Answer 2: user.name=Sandro Nuakey
	  user.email=sn261818@ohio.edu
Answer 3: GIT-ADD(1)                                  Git Manual                                  GIT-ADD(1)

NAME
       git-add - Add file contents to the index

SYNOPSIS
       git add [--verbose | -v] [--dry-run | -n] [--force | -f] [--interactive | -i] [--patch | -p]
                 [--edit | -e] [--[no-]all | --[no-]ignore-removal | [--update | -u]]
                 [--intent-to-add | -N] [--refresh] [--ignore-errors] [--ignore-missing] [--renormali
                 [--chmod=(+|-)x] [--] [<pathspec>...]

DESCRIPTION
       This command updates the index using the current content found in the working tree, to
       prepare the content staged for the next commit. It typically adds the current content of
       existing paths as a whole, but with some options it can also be used to add content with
       only part of the changes made to the working tree files applied, or remove paths that do
       not exist in the working tree anymore.

       The "index" holds a snapshot of the content of the working tree, and it is this snapshot
       that is taken as the contents of the next commit. Thus after making any changes to the
       working tree, and before running the commit command, you must use the add command to add
       any new or modified files to the index.

       This command can be performed multiple times before a commit. It only adds the content of
       the specified file(s) at the time the add command is run; if you want subsequent changes
       included in the next commit, then you must run git add again to add the new content to the
       index.

       The git status command can be used to obtain a summary of which files have changes that are
       staged for the next commit.

       The git add command will not add ignored files by default. If any ignored files were
       explicitly specified on the command line, git add will fail with a list of ignored files.
       Ignored files reached by directory recursion or filename globbing performed by Git (quote
       your globs before the shell) will be silently ignored. The git add command can be used to
       add ignored files with the -f (force) option.

       Please see git-commit(1) for alternative ways to add content to a commit.

OPTIONS
       <pathspec>...
           Files to add content from. Fileglobs (e.g.  *.c) can be given to add all matching
           files. Also a leading directory name (e.g.  dir to add dir/file1 and dir/file2) can be
           given to update the index to match the current state of the directory as a whole (e.g.
           specifying dir will record not just a file dir/file1 modified in the working tree, a
           file dir/file2 added to the working tree, but also a file dir/file3 removed from the
           working tree. Note that older versions of Git used to ignore removed files; use
           --no-all option if you want to add modified or new files but ignore removed ones.

           For more details about the <pathspec> syntax, see the pathspec entry in gitglossary(7).

       -n, --dry-run
           Don’t actually add the file(s), just show if they exist and/or will be ignored.

 Manual page git-add(1) byte 3485/18120 19% (press h for help or q to quit)

Answer 4: On branch master

	  No commits yet

	  Untracked files:
  	  (use "git add <file>..." to include in what will be committed)

	    README.md
	    answers.md

	  nothing added to commit but untracked files present (use "git add" to track)

Answer 5: On branch master

	  No commits yet

	  Changes to be committed:
  	    (use "git rm --cached <file>..." to unstage)

		new file:   README.md

	  Untracked files:
  	    (use "git add <file>..." to include in what will be committed)

		answers.md

Answer 6: On branch master

	  No commits yet

	  Changes to be committed:
  	    (use "git rm --cached <file>..." to unstage)

		new file:   README.md
		new file:   answers.md
Answer 7: On branch master
	   nothing to commit, working tree clean
Answer 8: 
commit 211f0ac0c1b0c245a475bae4ac60f38bfa6a14ca (HEAD -> master)
Author: Sandro Nuakey <sn261818@ohio.edu>
Date:   Fri Jan 21 14:43:42 2022 -0500

    Initial commit
Answer 9:
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   answers.md

no changes added to commit (use "git add" and/or "git commit -a")

Answer 10: No, the changes aren't present in the local copy.
Answer 11:
To https://github.com/sandronuakey37/git-lab.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/sandronuakey37/git-lab.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Answer 12: Yes, the changes are now in the local file
Answer 13: .  ..  .git  .gitignore  README.md








