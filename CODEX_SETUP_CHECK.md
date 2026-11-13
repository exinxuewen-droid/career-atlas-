# Career Atlas 云端 GitHub 发布能力测试

测试日期：2026-11-13（Asia/Shanghai）。

## 范围

- 目标仓库：`exinxuewen-droid/career-atlas-`，目标集成分支：`main`。
- 目标网站：https://cheerful-truffle-a6555a.netlify.app/
- 本次仅新增本说明文件，不修改网站页面，不删除任何文件。
- 已读取首页及四个专业页面：电子信息工程、生物医学工程、机械工程、生物工程；页面均存在，HTML 标题与专业对应。

## 当前验证结果

- GitHub HTTPS Git 读取成功，测试开始时远程 main 为 `aa5c26a3142a59eef1129795fd502f3b50d6fdd5`。
- 预期 GitHub 身份为 `exinxuewen-droid`，但身份 API 请求被环境网络策略以 403 拦截，尚未确认实际认证身份。仓库所有者及 Git 提交作者不能代替认证身份验证。
- 当前网络允许 github.com 的 Git 操作，但未允许 api.github.com 或目标 Netlify 网站。GitHub CLI 的身份检查同样被拦截，其 token 无效提示不能单独证明平台 Git 代理凭据无效。
- 优先使用独立测试分支并创建 PR，不自动合并。分支推送、PR 创建及最终提交标识以执行后的远程核对结果为准；推送预检不是实际写入成功的证明。
- Netlify 网站访问被网络策略以 403 拦截，尚不能确认部署触发或发布成功。需要放行目标站点并查询与提交对应的部署记录，不能以 Git 推送成功代替部署成功。

本说明记录测试范围与已知限制，不包含凭据。
