# Contributing to Seikode

All repositories in Seikode-LLC follow the same rules. The full engineering and
UI/UX guidelines are in the private
[handbook](https://github.com/Seikode-LLC/handbook) (organization members only).

Seikode-LLC 下所有仓库遵守同一套规则。完整的工程规范和 UI/UX 规范见私有仓库
[handbook](https://github.com/Seikode-LLC/handbook)（仅组织成员可见）。

## Hard rules / 硬性规定

1. **Every change goes through a pull request.** Direct pushes to the default
   branch are blocked. / **所有改动必须通过 PR 合并**，默认分支禁止直接 push。
2. **Checks must pass.** The `policy / pr-policy` check and each repository's
   own CI must be green. / **检查必须全部通过**：`policy / pr-policy` 以及仓库自己的 CI。
3. **The owner approves every merge.** Code owners review is required; approval
   is dismissed when new commits are pushed. / **每次合并须经负责人批准**，
   PR 有新提交后旧的批准自动作废。
4. **Human authors only.** No AI co-author trailers or "Generated with" footers
   in commits. / **提交只署本人名字**，不得带 AI 合著者署名。
5. **No secrets in Git.** Use environment variables and `.env` files that are
   ignored by Git. / **密钥不进 Git**，用环境变量和被忽略的 `.env`。

## Workflow / 流程

```bash
git switch -c feat/short-name        # branch from the default branch / 从默认分支拉新分支
# ... commit ...
git push -u origin feat/short-name
gh pr create --fill                  # then fill in the template / 然后按模板填写
```
