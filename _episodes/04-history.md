We've been adding one line at a time to `README.md`, so it's easy to track our
let's make another change to `README.md`.
$ nano README.md
$ cat README.md
# about your new image collection
The `cats-human-situations.csv` file contains metadata for three image objects. The original metadata from the source institutions has been abbreviated and made messier so you have something to clean up!
Image credits:
- The black cat, March 1896 (http://ark.digitalcommonwealth.org/ark:/50959/w0892s818). Courtesy Boston Public Library via Digital Commonwealth.
- Puzzums in costume (http://photos.lapl.org/carlweb/jsp/DoSearch?index=z&databaseID=968&terms=0000068045). Courtesy Los Angeles Public Library.
- A Xmas shopper (http://digitalcollections.nypl.org/items/510d47e1-43b5-a3d9-e040-e00a18064a99). Courtesy New York Public Library.

The images are in the `images/` subdirectory of this repository.
If you would like, you can also put images of dogs and hexagonal software logos here.
The real goodness in all this is when you can refer to previous commits.
We do that by adding `~1` to refer to the commit one before `HEAD`.
$ git diff HEAD~1 README.md
$ git diff HEAD~2 README.md
diff --git a/README.md b/README.md
index acbad52..0e44dff 100644
--- a/README.md
+++ b/README.md
@@ -6,3 +6,6 @@ Image credits:
 - The black cat, March 1896 (http://ark.digitalcommonwealth.org/ark:/50959/w0892s818). Courtesy Boston Public Library via Digital Commonwealth.
 - Puzzums in costume (http://photos.lapl.org/carlweb/jsp/DoSearch?index=z&databaseID=968&terms=0000068045). Courtesy Los Angeles Public Library.
 - A Xmas shopper (http://digitalcollections.nypl.org/items/510d47e1-43b5-a3d9-e040-e00a18064a99). Courtesy New York Public Library.
+
+The images are in the `images/` subdirectory of this repository.
+If you would like, you can also put pictures of dogs and hexagonal software logos here.

$ git show HEAD~2 README.md
commit 1ecad50e9ee2f30d9de4f3854af5faa6c5231fa3
Author: Catsy Cline <ccline@pawston.edu>
Date:   Thu Oct 26 09:54:31 2017 -0700
    add notes on metadata

diff --git a/README.md b/README.md
new file mode 100644
index 0000000..acbad52
--- /dev/null
+++ b/README.md
@@ -0,0 +1,8 @@
+# about your new image collection
+
+The `cats-human-situations.csv` file contains metadata for three image objects. The original metadata from the source institutions has been abbreviated and made messier so you have something to clean up!
+
+Image credits:
+- The black cat, March 1896 (http://ark.digitalcommonwealth.org/ark:/50959/w0892s818). Courtesy Boston Public Library via Digital Commonwealth.
+- Puzzums in costume (http://photos.lapl.org/carlweb/jsp/DoSearch?index=z&databaseID=968&terms=0000068045). Courtesy Los Angeles Public Library.
+- A Xmas shopper (http://digitalcollections.nypl.org/items/510d47e1-43b5-a3d9-e040-e00a18064a99). Courtesy New York Public Library.
`1ecad50e9ee2f30d9de4f3854af5faa6c5231fa3`,
$ git diff 1ecad50e9ee2f30d9de4f3854af5faa6c5231fa3 README.md
diff --git a/README.md b/README.md
index acbad52..0e44dff 100644
--- a/README.md
+++ b/README.md
@@ -6,3 +6,6 @@ Image credits:
 - The black cat, March 1896 (http://ark.digitalcommonwealth.org/ark:/50959/w0892s818). Courtesy Boston Public Library via Digital Commonwealth.
 - Puzzums in costume (http://photos.lapl.org/carlweb/jsp/DoSearch?index=z&databaseID=968&terms=0000068045). Courtesy Los Angeles Public Library.
 - A Xmas shopper (http://digitalcollections.nypl.org/items/510d47e1-43b5-a3d9-e040-e00a18064a99). Courtesy New York Public Library.
+
+The images are in the `images/` subdirectory of this repository.
+If you would like, you can also put pictures of dogs and hexagonal software logos here.
$ git diff 1ecad50 README.md
diff --git a/README.md b/README.md
index acbad52..0e44dff 100644
--- a/README.md
+++ b/README.md
@@ -6,3 +6,6 @@ Image credits:
 - The black cat, March 1896 (http://ark.digitalcommonwealth.org/ark:/50959/w0892s818). Courtesy Boston Public Library via Digital Commonwealth.
 - Puzzums in costume (http://photos.lapl.org/carlweb/jsp/DoSearch?index=z&databaseID=968&terms=0000068045). Courtesy Los Angeles Public Library.
 - A Xmas shopper (http://digitalcollections.nypl.org/items/510d47e1-43b5-a3d9-e040-e00a18064a99). Courtesy New York Public Library.
+
+The images are in the `images/` subdirectory of this repository.
+If you would like, you can also put pictures of dogs and hexagonal software logos here.
$ nano README.md
$ cat README.md
Dogs and hexagonal software logos as data.
	modified:   README.md
$ git checkout HEAD README.md
$ cat README.md
# about your new image collection

The `cats-human-situations.csv` file contains metadata for three image objects. The original metadata from the source institutions has been abbreviated and made messier so you have something to clean up!

Image credits:
- The black cat, March 1896 (http://ark.digitalcommonwealth.org/ark:/50959/w0892s818). Courtesy Boston Public Library via Digital Commonwealth.
- Puzzums in costume (http://photos.lapl.org/carlweb/jsp/DoSearch?index=z&databaseID=968&terms=0000068045). Courtesy Los Angeles Public Library.
- A Xmas shopper (http://digitalcollections.nypl.org/items/510d47e1-43b5-a3d9-e040-e00a18064a99). Courtesy New York Public Library.

The images are in the `images/` subdirectory of this repository.
$ git checkout 6b5b051 README.md
$ cat README.md
# about your new image collection

The `cats-human-situations.csv` file contains metadata for three image objects. The original metadata from the source institutions has been abbreviated and made messier so you have something to clean up!

Image credits:
- The black cat, March 1896 (http://ark.digitalcommonwealth.org/ark:/50959/w0892s818). Courtesy Boston Public Library via Digital Commonwealth.
- Puzzums in costume (http://photos.lapl.org/carlweb/jsp/DoSearch?index=z&databaseID=968&terms=0000068045). Courtesy Los Angeles Public Library.
- A Xmas shopper (http://digitalcollections.nypl.org/items/510d47e1-43b5-a3d9-e040-e00a18064a99). Courtesy New York Public Library.

The images are in the `images/` subdirectory of this repository.

On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)

	cats-human-situations.csv

nothing added to commit but untracked files present (use "git add" to track)
$ git checkout -f master README.md
> $ git checkout 6b5b051 README.md
> to revert `README.md` to its state after the commit `6b5b051`.
> If you forget `README.md` in that command, Git will tell you that "You are in
> What is the output of cat CONTRIBUTING.md at the end of this set of commands?
> $ cd cats-as-data
> $ nano CONTRIBUTING.md #input the following text: Please submit changes in a Pull Request
> $ git add CONTRIBUTING.md
> $ nano CONTRIBUTING.md #add the following text: Don't forget cat images, please.
> $ git commit -m "Add CONTRIBUTING.md to project"
> $ git checkout HEAD CONTRIBUTING.md
> $ cat CONTRIBUTING.md #this will print the contents of CONTRIBUTING.md to the screen
> Please submit changes in a Pull Request
> Don't forget cat images, please.
> Please submit changes in a Pull Request
> Don't forget cat images, please.
> Error because you have changed CONTRIBUTING.md without committing the changes
> > $ cd cats-as-data
> > Enters into the 'cats-as-data' directory
> > $ nano CONTRIBUTING.md #input the following text: Please submit changes in a Pull Request
> > $ git add CONTRIBUTING.md
> > $ nano CONTRIBUTING.md #add the following text: Don't forget cat images, please.
> > $ git commit -m "Add CONTRIBUTING.md to project"
> > The changes that were staged (Please submit changes in a Pull Request) have been committed. The changes that were not staged (Don't forget cat images, please.) have not. Our local working copy is different than the copy in our local repository.
> > $ git checkout HEAD CONTRIBUTING.md
> > $ cat CONTRIBUTING.md #this will print the contents of CONTRIBUTING.md to the screen
> > If we print CONTRIBUTING.md we will get answer 2.
> Consider this command: `git diff HEAD~3 README.md`. What do you predict this command
> Try another command, `git diff [ID] README.md`, where [ID] is replaced with
> Make a change to `README.md`, add that change, and use `git checkout` to see if
> Imagine the `cats-as-metadata` project has more than 50 files.
> You would like to find a commit with specific text in `README.md` is modified.
> Recall that the `git diff` command allow us to explore one specific file,
> e.g. `git diff README.md`. We can apply the similar idea here.
> $ git log README.md
> $ git log --patch README.md
> $ git log --patch HEAD~3 *.md