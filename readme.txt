学习git：创建版本库一节，git add 文件名；git commit -m "xxx"
git status 告诉当前仓库状态，若有修改但没提交，则可以用git diff xxx来查看上次修改的内容
提交修改和添加步骤一样git add 然后git commit;
版本回退，git log显示最近到最远的提交日志，--pretty=oneline可以简化显示，git的提交id使用SHA1计算出来的，每提交一个新版本，git把
他们自动串成一条时间线，对于本机，HEAD表示当前版本（对应一个commit id）上一个版本是HEAD^,上上个是
HEAD^^,100个表示成HEAD~100。git reset --hard HEAD^可以让当前文件回到上一个版本，并且最新版本的log也看不到了
当可以直接用git reset --hard 1094a回到指定的版本，那串数字表示commit id，不必写全。git reflog查看每一次命令
