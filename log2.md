```git
HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (weeeeeel)
$ ll
total 6
-rw-r--r-- 1 HmLa 197609 663 7月  16 10:33 lessonLog.md
-rw-r--r-- 1 HmLa 197609  50 7月  16 09:37 text.md
-rw-r--r-- 1 HmLa 197609  28 7月  16 10:30 tt.md

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (weeeeeel)
$ vim tt.md

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (weeeeeel)
$ git add .
warning: LF will be replaced by CRLF in tt.md.
The file will have its original line endings in your working directory

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (weeeeeel)
$ git commit .
warning: LF will be replaced by CRLF in tt.md.
The file will have its original line endings in your working directory
[weeeeeel e642503] asdasdasdasd
 1 file changed, 2 insertions(+)

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (weeeeeel)
$ git checkout master
Switched to branch 'master'

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master)
$ vim tt.md

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master)
$ git add commit .
fatal: pathspec 'commit' did not match any files

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master)
$ git add .

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master)
$ git commit -m "asdmaster"
[master fc25df3] asdmaster
 1 file changed, 2 insertions(+)

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master)
$ git checkout weeeeeel
Switched to branch 'weeeeeel'

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (weeeeeel)
$ git checkout master
Switched to branch 'master'

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master)
$ git merge weeeeeel
Auto-merging tt.md
CONFLICT (content): Merge conflict in tt.md
Automatic merge failed; fix conflicts and then commit the result.

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master|MERGING)
$ git diff
diff --cc tt.md
index c53a9b4,f01b7d5..0000000
--- a/tt.md
+++ b/tt.md
@@@ -1,6 -1,7 +1,11 @@@
  dfg
++<<<<<<< HEAD
 +++>>>>>>>>>>>>>>>> sdfasdasdasdasd
++=======
+ ++>>>>>>>>>>> Head
++>>>>>>> weeeeeel
  sersg
+ ++<<<<<<<<<<<<defv
  erg
  red
  ger

HmLa@HYKMH MINGW64 /d/LESSON/HomeWorks/gitss (master|MERGING)
$
```
