1. 组长：新建github仓库，复制ssh仓库地址
2. 组长：git clone "复制的地址"
3. 组长：git remote add origin '复制的地址'
4. 组长：git push -u origin master
5. 组长：git checkout -b dev
6. 组长：git push -u origin dev

7. 组员小智：git clone "复制的地址"
8. 组员小智：git checkout -b dev origin/dev
9. 组员小智：git checkout -b xiaozhi dev
10. 组员小智：git status, git add, git commit
11. 组员小智: git checkout dev
12. 组员小智：git pull
13. 组员小智： git merge xiaozhi
14. 组员小智： git push
15. 组员小智： git checkout xiaozhi
16. 组员小智： git merge xiaozhi
```
此时如果出现
# Please enter a commit message to explain why this merge is necessary,
# especially if it merges an updated upstream into a topic branch。
# lines starting with "#" will be ignored, and an empty message aborts the commit

// 可以按 Esc 退出键，输入 :wq, 然后按下回车键即可
```
17. 组员小智： git push
18. 组员小狒：git clone "复制的地址"
19. 组员小狒：git checkout -b dev origin/dev
20. 组员小狒：git checkout -b xiaofei dev
21. 组员小狒：git status, git add, git commit
22. 组员小狒：git checkout devs
23. 组员小狒：git pull 
24. 组员小狒：git merge xiaofei

```
// 此时如果出现冲突
<<<<<<< HEAD
// 从HEAD到下面的====之间的代码是你拉取的别的组员的代码
function a () {
	console.log('a')
}
=======
// 从======到下面的>>>>>之间的代码是小狒修改的代码
>>>>>>> xiaofei

// 需要小狒和小智商量，保留小智的还是保留小狒的，还是两个人的都要保留一部分。手动改好代码后，执行
git add '冲突的文件名'
git commit -m '解决冲突'
接着往下执行
```

25. 组员小狒：git push

23. 组长：git checkout -b release dev
24. 组长：git push -u origin release
25. 组员小智：git checkout -b release origin/release
27. 组员小智：git checkout xiaozhi
28. 组员小智：git merge release
29. 组员小智：git status, git add, git commit -m "修改bug0001"
30. 组员小智：git checkout release
31. 组员小智：git pull
32. 组员小智：git merge xiaozhi
33. 组员小智：git push
34. 组员小智：git checkout xiaozhi
35. 组员小智：git merge release

