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
14. 组员小智： git push