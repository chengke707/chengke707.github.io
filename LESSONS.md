# 项目总结：程柯个人主页部署全记录

> 日期：2026-07-11
> 网址：https://chengke707.github.io/

---

## 一、最终成果

| 项目 | 内容 |
|------|------|
| 网页 | 单文件 index.html（38KB，1200+行），毛玻璃卡片、三色分区、滚动动画 |
| 功能 | 性格画像、技能进度条、证书卡片、微信弹窗、邮箱复制 |
| 托管 | GitHub Pages（免费、稳定、无需实名） |
| 网址 | `https://chengke707.github.io/` |

---

## 二、正确流程（以后这样做）

### 🏆 最快路径：GitHub Pages + 网页上传

```
① 注册 GitHub 账号（1 次）
② 创建仓库：<用户名>.github.io
③ 把 index.html 拖到仓库页面 → Commit changes
④ 等 30 秒，网站上线
```

**就这么简单。不需要 Git、不需要终端、不需要 SSH。**

---

## 三、踩过的坑

| 坑 | 原因 | 教训 |
|-----|------|------|
| **Gitee Pages 要实名认证** | Gitee 国内政策要求 | ❌ 别用 Gitee，用 GitHub |
| **deepseek 审核宕机** | Claude Code 云端服务故障 | 终端命令不可靠时，直接用网页上传 |
| **Git SSH 密钥折腾** | 每次操作都被审核拦截 | 网页上传根本不需要密钥 |
| **密码暴露风险** | 多次尝试在命令中传密码 | 永远用 SSH Key 或网页上传 |

---

## 四、以后部署新网站的模板操作

### 新项目 Checklist

```
□ 1. 写好 index.html
□ 2. 打开 github.com，创建新仓库 <名字>
□ 3. 仓库 Settings → Pages → Source: main → Save
□ 4. Add file → Upload files → 拖入 index.html → Commit
□ 5. 等 30 秒，访问 https://<用户名>.github.io/<仓库名>/
```

### 更新已有网站

```
□ 1. 修改本地的 index.html
□ 2. 打开 GitHub 仓库页面
□ 3. 找到 index.html → 点编辑（铅笔图标）
□ 4. 全选删除 → 粘贴新内容 → Commit
□ 5. 刷新网址
```

---

## 五、你的账号信息（妥善保管）

| 平台 | 用户名 | 用途 |
|------|--------|------|
| GitHub | `chengke707` | 托管网站 |
| Gitee | `riding-the-winds-to-greatness` | 备用 |

---

## 六、核心原则

> **网页上传 > Git 推送**
>
> 能用网页拖拽解决的，永远不要开终端。

> **GitHub > Gitee**
>
> GitHub Pages 不需要实名认证，自动部署，服务稳定。

> **单文件 > 多文件**
>
> 一个 index.html 包含所有 CSS/JS，部署只需上传一个文件。

---

## 七、下次你可以怎么做

1. 在本地写/改好 index.html
2. 打开 GitHub 仓库页面
3. 把文件拖进去
4. 完成

**全程不需要我参与，30 秒上线。** 遇到复杂需求再找我写代码，部署你自己就能搞定。
