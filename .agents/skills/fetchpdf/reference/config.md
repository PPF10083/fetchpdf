# 环境配置

1. 在用户指定或当前项目已有的 Python 环境中安装 `fetchpdf` 包。若 Agent 不清楚哪个环境，请直接询问用户。
2. 参照 [配置示例](../reference/.env.example)，默认创建 `.env.local`：
```
cp /path/to/reference/.env.example ./.env.local
```
3. 至少填写让用户填写 `.env.local` 的 `EMAIL` 和 `CROSSREFEMAIL`, 其余密钥均为按需配置。

注：配置 `.env.local` 有助于：
1. 提升获取速度与稳定性
2. 扩大可访问源
