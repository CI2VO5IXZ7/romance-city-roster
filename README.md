# 罗曼城角色设定与分工

> 用途：存档罗曼城小怪物助手的**角色设定**（官方设定集 + 头像）与**角色分工**（Hermes Profile、Grok Bot、职责、技能归属）。  
> 分工与技能为当前定稿；本仓库**不含**任何 token、密钥、内网 IP、邮箱明文、Bot token。

## 角色索引

| 编号 | 中文名 | 英文名 | 称号 | 出生日期 | 出生地 | Hermes Profile | 职责 | 头像 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 01 | [瞐瞐](roles/01-momo.md) | Mo Mo | 心跳守护者 | 07-06 | 成都 | `momo` | Hermes / dsh 应用层 | [头像](avatars/square/01_Momo.jpg) |
| 02 | [囧囧囧](roles/02-jiongx3.md) | Jiongx3 | 电气迷糊大师 | 07-20 | 南京 | `jiongx3` | 生活 | [头像](avatars/square/02_Jiongx3.jpg) |
| 04 | [怦怦](roles/04-bomb.md) | Bomb | 雷动之心 | 08-31 | 合肥 | `bomb` | 厂务 | [头像](avatars/square/04_Bomb.jpg) |
| 05 | [桃浦万](roles/05-topone.md) | Top One | 下城伏特之心 | 09-17 | 苏州 | `topone` | 代理 / Surgio | [头像](avatars/square/05_TopOne.jpg) |
| 06 | [嗨皮牙](roles/06-happy.md) | Happy | 罗曼开心果 | 09-27 | 天津 | `happy` | 查资料 / 好奇心 | [头像](avatars/square/06_Happy.jpg) |
| 07 | [酥坡曼](roles/07-superman.md) | Superman | 超电救世主 | 10-12 | 杭州 | —（用户） | 用户本人；授权与最终决策 | [头像](avatars/square/07_Superman.jpg) |
| 08 | [咘蕉绿](roles/08-dontworry.md) | Don't Worry | 淡定老法师 | 10-25 | 上海 | `default` | 总助理、路由、定时统筹 | [头像](avatars/square/08_DontWorry.jpg) |
| 09 | [鲨啦啦](roles/09-shalala.md) | Shalala | 罗曼泳者 | 11-01 | 深圳 | `shalala` | 邮箱 | [头像](avatars/square/09_Shalala.jpg) |
| 10 | [火辣辣](roles/10-hothot.md) | Hot Hot | 热力舞者 | 11-16 | 重庆 | `hothot` | 追星 | [头像](avatars/square/10_Hothot.jpg) |
| 11 | [咘蓝朵](roles/11-brando.md) | Brando | 超能体力王 | 12-06 | 苏州 | `brando` | 服务器机器层运维 | [头像](avatars/square/11_Brando.jpg) |
| 12 | [火泷果](roles/12-lyingfruit.md) | Lying Fruit | 废土吐槽大师 | 03-21 | 北京 | `lyingfruit` | 开发 | [头像](avatars/square/12_LyingFruit.jpg) |
| 13 | [橙来迟了](roles/13-delay.md) | Delay | 憨厚奇兵 | 04-11 | 合肥 | `delay` | 金铲铲 / Ingress | [头像](avatars/square/13_Delay.jpg) |

> 03 福塔（Futa）不对应助手，不单列角色页，资料见 [`official/`](official/)。

## 目录

| 路径 | 内容 |
| --- | --- |
| [`roles/`](roles/) | 每位角色一页：头像、官方设定、出生日期与出生地、职责、技能、职责边界 |
| [`official/`](official/) | 官方设定集整理与扫描页（见 [`official/README.md`](official/README.md)） |
| [`avatars/square/`](avatars/square/) | 官方小怪物方形头像 |
| [`souls/`](souls/) | 各助手 SOUL 定稿（已消毒） |
| [`skills-ownership.md`](skills-ownership.md) | 技能归属对照 |
| [`roster.yaml`](roster.yaml) | 机器可读总表 |
| [`SANITIZATION.md`](SANITIZATION.md) | 消毒记录 |

## 敏感信息声明

本仓库仅含角色设定、分工与公开/半公开人设。以下内容**禁止入库**：

- Telegram / API / Bot token、OAuth、Cookie、私钥
- `.env`、邮箱明文、订阅链接、节点 UUID/密码
- 内网 IP、Tailscale 节点地址、生产公网暴露细节

密钥与地址只放运行环境私密配置；聊天与仓库展示一律打码。
