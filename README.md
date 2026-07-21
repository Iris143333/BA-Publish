# BA Lineage Explorer Demo

这是一个只读的数据血缘演示站点。页面和元数据均由 `docs/` 提供，可直接部署到 GitHub Pages。

## 本地运行

在仓库根目录执行：

```bash
python3 -m http.server 8765 --bind 0.0.0.0
```

然后打开：

```text
http://127.0.0.1:8765/docs/index.html
```

## GitHub Pages

仓库推送后，在 GitHub 仓库中打开：

`Settings → Pages → Build and deployment → Deploy from a branch`

选择 `main` 分支和 `/docs` 目录。站点地址通常为：

```text
https://iris143333.github.io/BA-Publish/
```

## 发布内容

- `docs/index.html`：页面入口
- `docs/styles.css`：页面样式
- `docs/global_app.js`：血缘交互逻辑
- `docs/data/metadata.json`：对象和关系元数据
- `docs/data/field_lineage_web.json`：字段血缘数据
- `docs/data/field_explanation_catalog.json`：字段解释数据

本仓库当前使用未脱敏数据；发布为公开仓库或开启 GitHub Pages 后，访问者可下载这些 JSON 文件并查看其中的 SQL、对象名称和业务解释。
