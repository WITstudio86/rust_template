# rust template

cargo make 可以实现定义多个子指令 , 并将他们组合,配置依赖 , 轻松的组合成为很多不同的自动化脚本

## init

```bash
$ cargo install --force cargo-make
$ cargo make check
```

## changelog 模板

```toml
    # 跳过
    { message = "\\[skip", skip = true },
    # feat 开头放入特性分类
    { message = "^feat", group = "feat" },
    # fix 开头放入 bug 修复分类
    { message = "^fix", group = "fix bug" },
    # doc 开头放入文档分类
    { message = "^doc", group = "document" },
    # perf 开头放入性能分类
    { message = "^perf", group = "perf" },
    # refactor 放入重构分类
    { message = "^refactor", group = "refactor" },
    # style 开头放入样式分类
    { message = "^style", group = "style" },
    # revert 放入还原复原分类
    { message = "^revert", group = "revert" },
    # test 放入测试分类
    { message = "^test", group = "tests" },
    # 以 chore: 开头，跳过这条提交
    { message = "^chore:", skip = true },
    # 包含 security 安全修复
    { body = ".*security", group = "security" },
    # 不匹配的其他内容归入 Other
    { message = ".*", group = "others" },
```
