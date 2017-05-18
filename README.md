# commit fix test

# this is test by yuu

- hoge

## first content
- hoge
- fuga

## second content
- hoge
- fuga

## work log

```
[yit@localhost commit_fix_test (master)]$ git co -b merge_commits_branch
Switched to a new branch 'merge_commits_branch'
[yit@localhost commit_fix_test (merge_commits_branch)]$ git log1
f7a704c31aa66e720e0fc0e6a89007abbef1ae78 add second content
058b0424128ec2390649aa98b59f91fc299a9cb3 add first contents
3ea4eee95f0bcc66e1e90219c31c5e3966323a92 add title at README
8d87c10085246757231a360eb1988155036c2082 first commit
[yit@localhost commit_fix_test (merge_commits_branch)]$ git rebase -i HEAD~3
[detached HEAD cd07865] add first and second content
 1 file changed, 8 insertions(+)
Successfully rebased and updated refs/heads/merge_commits_branch.
[yit@localhost commit_fix_test (merge_commits_branch)]$ git log1
cd0786564a03d260b0f992a6fc9f31a0ff81079d add first and second content
3ea4eee95f0bcc66e1e90219c31c5e3966323a92 add title at README
8d87c10085246757231a360eb1988155036c2082 first commit
```
