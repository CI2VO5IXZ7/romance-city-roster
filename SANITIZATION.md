# 消毒记录（SANITIZATION）

扫描时间：2026-10-22（Asia/Shanghai）  
范围：本资料包全树（含 `roles/`、`souls/`、`avatars/`、根目录 md/yaml）

## 查了什么

对文本文件用关键词 / 模式检索，至少覆盖：

- `token` / `api_key` / `secret` / `password` / `passwd` / `Bearer …`
- `sk-…`、`AKIA…`、PEM/OpenSSH 私钥头、`ssh-rsa`
- Telegram Bot token 形态（`Bot <digits>:<secret>`）
- 已知敏感域名形态、内网/公网 IPv4
- 常见邮箱明文（gmail / outlook / qq / 163 / icloud）
- 本机绝对路径（`/workspace/…`、`/home/box/…`）

并对 `souls/brando.SOUL.md` 人工检查主机清单。

## 处置

| 项 | 结果 |
| --- | --- |
| 明文 Bot / API token | 未发现 |
| 私钥 / PEM | 未发现 |
| 邮箱明文 | 未发现 |
| 内网 / 公网 IP | 未发现 |
| 订阅链接 / UUID / 密码 | 未发现 |
| brando 管机主机名清单 | **已改写**：具体主机名不入库，改为「酥坡曼指定的自有主机…」 |
| README / 归属表中的本机绝对路径 | **已去掉**，改为相对描述 |
| 「token / 密钥 / .env」字样 | 仅出现在**禁止泄露**的政策句中，无具体值 |

## 结论

**干净，可推私有空仓。**  
仍请推送前人工再扫一遍；运行环境密钥不要拷进本仓库。

## 已知非密钥残留（可接受）

- SOUL 中提及 Tailscale / SSH 作为职责描述（无节点地址）。
- Grok Bot agent UUID（公开于本体系 roster，非凭据）。
- 时区字符串 `Asia/Shanghai`。
