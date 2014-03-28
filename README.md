sample
======

Testing ground for git commands


Git workflow using commits


  1. Create a local branch and give it a descriptive name based on the issue

      * git checkout -b issue_name

  2. After making changes, commit them to the local branch

      * git commit -a

  3. To switch back to master branch

      * git checkout master
      * git status

         * You should not see commits from local branch


  4. To merge multiple commits into single

      * git rebase -i
      * Git will present an editor. Replace “pick” with “squash” for all but the first commit. This will merge all commits into the first one.




Common Git commands


   * Clone a repo

      * git clone [—depth 1] <repo>



   * Create/update a review board

      * git review create

      * git review update



   * View unpushed git commits


      * git log origin/master..HEAD




   * Discard (i.e. revert) a file:

      * git checkout — todo.txt




   * Update/sync submodules

      * git submodule update —init

      * git submodule sync




   * Sync with remote repo, and move your commit to the top

      * git pull —rebase



   * Remove all changes from a commit

      * git reset --soft 'HEAD^’



Applying a patch


   * show the status of what git apply will do


      * git apply —stat <path_to_patch>




   * show any errors git apply might encounter


      * git apply —check <path_to_patch>




   * apply the patch


      * git apply <path_to_patch>




