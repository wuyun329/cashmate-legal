---
AIGC:
    Label: "1"
    ContentProducer: 001191440300708461136T1XGW3
    ProduceID: 1d60355381afc33689aa6ecf0c6b4081_ef7f201ce48711f1a5ef525400638852
    ReservedCode1: B9kxImK5FM3pzla8c03B782mn3mSyadvoKArfd3yv5eQBAkJzT2sbTRet2FGh/V2s2Sg49gKnxUYk0Y+Gpd7VJBoaTu3am8/xDClLgvBrhphowI052+64JRYrxwalttYk4a7t78pKvtLlozkIWxmE2jZNloH8MnlA1LEIGQ1Q40C9ykE6ErnLFQZ1EA=
    ContentPropagator: 001191440300708461136T1XGW3
    PropagateID: 1d60355381afc33689aa6ecf0c6b4081_ef7f201ce48711f1a5ef525400638852
    ReservedCode2: B9kxImK5FM3pzla8c03B782mn3mSyadvoKArfd3yv5eQBAkJzT2sbTRet2FGh/V2s2Sg49gKnxUYk0Y+Gpd7VJBoaTu3am8/xDClLgvBrhphowI052+64JRYrxwalttYk4a7t78pKvtLlozkIWxmE2jZNloH8MnlA1LEIGQ1Q40C9ykE6ErnLFQZ1EA=
---

# cashmate-legal

CashMate 记账（iOS / Android）的隐私政策与支持页静态站，托管在 GitHub Pages，供 App Store Connect 填写「隐私政策 URL」与「支持 URL」。

仓库内只有三个文件，无构建步骤、无外部依赖（不引用外部字体、CDN、图片与任何统计脚本，纯内联 CSS），上传即可访问。

| 文件 | 用途 | 对应线上地址 |
| --- | --- | --- |
| `index.html` | 隐私政策页 | `https://<用户名>.github.io/cashmate-legal/` |
| `support.html` | 支持与联系页（含 5 条常见问题） | `https://<用户名>.github.io/cashmate-legal/support.html` |
| `README.md` | 本说明 | 不需要访问 |

内容口径：应用名 CashMate 记账，版本 1.0.1，开发者吴赟（Wu Yun），联系邮箱 wuyun329@agent.qq.com，更新日期与生效日期均为 2026 年 11 月 20 日。修改隐私政策正文时，需同时更新应用内 `src/legal.ts` 与 `D:\Dev\firstapp\docs\privacy.html`，三处保持一致。

## 部署步骤

1. 打开 GitHub 网页端，登录后点右上角 **+** → **New repository**。
2. 仓库名填 `cashmate-legal`，可见性选 **Public**（私有仓库的 Pages 需要付费方案，App Store 审核也必须能公开访问），不要勾选「Add a README file」，然后点 **Create repository**。
3. 进入新建的空仓库，点 **uploading an existing file**（或 **Add file → Upload files**），把本地这三个文件 `index.html`、`support.html`、`README.md` 一起拖进页面根目录（不要放进任何子文件夹），填一句提交说明后点 **Commit changes**。
4. 打开仓库的 **Settings** → 左侧 **Pages**。
5. 在 **Build and deployment** 的 **Source** 选择 **Deploy from a branch**，**Branch** 选 `main`、目录选 `/(root)`，点 **Save**。
6. 等待 1–2 分钟，刷新该 Pages 页面，顶部会出现提示「Your site is live at ...」，得到两个地址：
   - 隐私政策：`https://<用户名>.github.io/cashmate-legal/`
   - 支持页：`https://<用户名>.github.io/cashmate-legal/support.html`
7. 首次发布或后续改动通常 1–2 分钟内生效，个别网络下可能延迟到十几分钟；若仍显示 404，先确认文件名大小写完全一致（必须是 `index.html`），再等待几分钟重试。

## 填入 App Store Connect

在 App Store Connect 里打开 CashMate 记账这个 App，进入「App 信息」页：

- **隐私政策 URL** 填 `https://<用户名>.github.io/cashmate-legal/`
- **支持 URL** 填 `https://<用户名>.github.io/cashmate-legal/support.html`

两个地址都要能直接在浏览器打开（未登录状态、手机流量下也能访问）。填完保存后，建议用手机无痕窗口各打开一次，确认页面渲染正常、联系方式可点击。

同时把 **支持 URL** 一并填到「App 信息 → 支持 URL」后，App Store 商品页的「App 支持」入口才会生效；若审核人员需要联系开发者，会通过该页面上的邮箱 wuyun329@agent.qq.com 联系。

## 备注

- GitHub Pages 的域名是 `github.io`，中国大陆访问稳定性一般，审核期与上线后建议自测；如后续需要更稳定的访问，可把同一份文件原样迁移到任意支持静态托管的服务，URL 变更后记得同步更新 App Store Connect 中的两个字段。
- 页面为纯静态文件，不采集访问者信息、不加载任何第三方脚本，因此无需额外的 Cookie 声明。
- 若仓库名不是 `cashmate-legal`，上面的两个地址中的路径段要替换成实际仓库名。
*（内容由AI生成，仅供参考）*
