# rust template

## release_please

添加了 release_please 的支持 可以根据 commit 信息自动生成 release PR

cargo make 可以实现定义多个子指令 , 并将他们组合,配置依赖 , 轻松的组合成为很多不同的自动化脚本

## init

```bash
$ cargo install --force cargo-make
$ cargo make check
```

## changelog 模板

```toml
{"type": "feat", "section": "✨ Features"},
{"type": "fix", "section": "🐛 Bug Fixes"},
{"type": "chore", "section": "🔧 Maintenance"},
{"type": "refactor", "section": "🧼 Refactors"},
{"type": "docs", "section": "📝 Documentation"},
{"type": "test", "section": "🧪 Tests"}
```
