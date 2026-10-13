# tv-nodes

subs-check 跑在 GitHub Actions 上（每 6 小时一轮，跑完即退出，不长驻），
合并公开免费订阅源 → 测活 → 测速 → 按 IP 归属地重命名 → 推到 secret Gist。

- 不占用任何自建 VPS 流量，全部用 GitHub 免费 runner
- 输出：secret Gist（unlisted，知道 URL 才能取；删除 Gist = 总开关）
- 凭据通过 Actions Secrets 注入，不进仓库
