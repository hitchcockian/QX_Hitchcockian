# 🎯 Hitchcockian QX 配置合集

Quantumult X 综合配置，整合去广告、解锁、签到功能于一体。

## ✨ 功能特点

- **广告拦截** — 基于 blackmatrix7 的广告、劫持、隐私拦截规则，覆盖全面
- **应用解锁** — 集成 Curtinp118 的多个应用 VIP 解锁脚本
- **TikTok 解锁** — 支持日/韩/台/英/美多地区 TikTok 解锁
- **自动签到** — 京东、爱奇艺、B站、网易云等多平台签到支持
- **流媒体检测** — 内置流媒体解锁检测脚本
- **策略分组** — 完善的策略组配置，按需分流
- **DNS 优化** — 国内 DNS 服务器配置，提高访问速度

## 📂 文件结构

```
QX_Hitchcockian.conf        # 主配置文件（导入此文件即可）
hitchcockian.json            # 定时任务配置
rewrite/
├── Advertising.conf         # 广告拦截重写规则（含微博/知乎/B站/抖音/小红书）
└── Unlock.conf              # 应用解锁重写规则合集
rules/
├── Advertising.list         # 广告域名过滤规则
└── Direct.list              # 直连域名规则
unlock/
├── dandanvip.conf           # 蛋蛋不语 VIP 解锁
├── buding.conf              # 布丁锁屏解锁
├── caiyun.conf              # 彩云天气 VIP 解锁
├── dreamface.conf           # DreamFace AI 换脸解锁
├── nicegram.conf            # Nicegram 解锁
├── notability.conf          # Notability 解锁
├── glados.conf              # GLaDOS 自动签到
├── cmcc.conf                # 中国移动签到
├── nodeseek.conf            # NodeSeek 论坛签到
└── new-api.conf             # NewAPI 通用签到
tiktok/
├── TikTokJP.conf            # TikTok 日本
├── TikTokKR.conf            # TikTok 韩国
├── TikTokTW.conf            # TikTok 台湾
├── TikTokUK.conf            # TikTok 英国
└── TikTokUS.conf            # TikTok 美国
```

## 🚀 使用说明

### 方式一：直接导入主配置

1. 打开 Quantumult X
2. 点击右下角「风车」图标 → 配置文件
3. 点击「下载配置」
4. 输入配置地址: `https://raw.githubusercontent.com/hitchcockian/QX/main/QX_Hitchcockian.conf`
5. 点击「好」等待下载完成

### 方式二：手动导入

1. 将 `QX_Hitchcockian.conf` 复制到 Quantumult X 配置目录
2. 导入 `hitchcockian.json` 到任务管理
3. 根据需要启用对应的解锁/签到脚本

### 使用解锁脚本

1. 在 QX 中启用对应的重写规则
2. 确保已安装相应的脚本资源
3. 按脚本要求配置 Cookie（如有需要）
4. 部分解锁需要配置 MITM 证书

## 📝 更新日志

### v1.0.0 (2026-06-01)

- 初始版本发布
- 整合 blackmatrix7 完整规则集
- 集成 Curtinp118 所有解锁脚本
- 添加 TikTok 多地区解锁
- 配置自动签到任务列表

## 🙏 鸣谢

- [Tartarus2014/QuantumultX-Script](https://github.com/Tartarus2014/QuantumultX-Script) — TikTok 解锁规则
- [curtinp118/QuantumultX](https://github.com/curtinp118/QuantumultX) — 应用解锁脚本
- [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script) — 规则与重写
- [KOP-XIAO/QuantumultX](https://github.com/KOP-XIAO/QuantumultX) — 资源解析及流媒体检测
- [chavyleung/scripts](https://github.com/chavyleung/scripts) — 签到脚本
- [NobyDa/Script](https://github.com/NobyDa/Script) — 京东签到脚本
- [dompling/Script](https://github.com/dompling/Script) — 签到脚本
