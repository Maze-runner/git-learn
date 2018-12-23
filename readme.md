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
14. 此时如果出现
```
# Please enter a commit message to explain why this merge is necessary,
# especially if it merges an updated upstream into a topic branch。
# lines starting with "#" will be ignored, and an empty message aborts the commit
```s
可以按 Esc 退出键，输入 :wq, 然后按下回车键即可
14. 组员小智： git push
15. 组员小智： git checkout xiaozhi
16. 组员小智： git merge xiaozhi
14. 组员小智： git push
15. 组员小狒：git clone "复制的地址"
16. 组员小狒：git checkout -b dev origin/dev
17. 组员小狒：git checkout -b xiaofei dev
18. 组员小狒：git status, git add, git commit
19. 组员小狒：git checkout dev
20. 组员小狒：git pull 
21. 组员小狒：git merge xiaofei
22. 组员小狒：git push
