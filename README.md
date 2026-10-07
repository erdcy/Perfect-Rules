# **Perfect Rules**
## ✈️推荐机场
[点击：九云机场8折优惠](https://n0de.jiuyyq.com)
专属优惠码：TowpY74S
- 高性能海外机场，海外团队，无跑路风险
- 集群负载均衡设计，高速专线，极低延迟，无视晚高峰，4K 秒开
- ⭐19.9元 500G，中秋限时优惠⭐
- ⭐29.9元1000G，中秋显示优惠⭐
- 优惠套餐每月仅需 6 元，150G 流量，年付 8 折
- 解锁流媒体及 ChatGPT

**阿尔忒弥斯实验室维护的代理分流配置方案。**

## **🚀 快速开始**

如果你是第一次使用 Perfect Rules，建议按照以下顺序选择：

**① Clash Mi → ② Clash / Mihomo → ③ V2rayN**

| **支持客户端** | **版本** | **客户端** | **功能**              | **配置文件**                                              | **使用方式**             | **教程视频**                 |
| -------------- | -------- | ---------- | --------------------- | --------------------------------------------------------- | ------------------------ | ---------------------------- |
| Shadowrocket   | 3.0      | 苹果端     | 完美分流/DNS防泄露    | [`perfect_rules.conf`](./Shadowrocket/perfect_rules.conf) | 一键导入                 | https://youtu.be/zppJJyy6BYo |
| FlClash        | 3.0      | 全平台     | 完美分流/DNS防泄露    | [`FlClash.js`](./Clash/FlClash.js)                        | 一键导入                 | https://youtu.be/7RXy43TpjTs |
| **Clash Mi**   | 3.0      | 全平台     | 完美分流 / DNS 防泄漏 | [`Clash_mi.js`](./Clash/Clash_mi.js)                      | 一键导入                 | https://youtu.be/jmJiyDSmZE0 |
| Clash / Mihomo | 3.0      | PC         | 完美分流 / DNS 防泄漏 | [`Clash_merge.yaml`](./Clash/Clash_merge.yaml)            | 复制粘贴（见下方）       | https://youtu.be/2A2SdHP_NKA |
| V2rayN         | 2.0      | PC         | 完美分流              | [`V2rayN.json`](./V2rayN.json)                            | 下载文件后配置（见下方） | https://youtu.be/eaTmKWPyVG4 |

**推荐：** 如果你希望在**不同设备上使用统一的**分流规则，并同时解决 DNS 泄漏问题，可以优先选择 **Clash Mi 3.0**。

------

## Shadowrocket 3.0 ：完美分流 + DNS防泄漏 ——一键配置

macOS和iOS端的Shadowrocket可以使用项目提供的[`perfect_rules.conf`](./Shadowrocket/perfect_rules.conf)，一键导入即可使用。

#### **远程配置地址**

**GitHub Raw：**

```text
https://github.com/n0de-sudo/Perfect-Rules/raw/refs/heads/main/Shadowrocket/perfect_rules.conf
```

## **① ⭐ Clash Mi 3.0：完美分流 + DNS 防泄漏——懒人版**

## FlClash 3.0：完美分流 + DNS防泄漏——一键配置

FlClash 用户可以使用项目提供的[`FlClash.js`](./Clash/FlClash.js)，一键导入完整的 Perfect Rules 配置。

目前FlClash支持多平台（仅iOS不支持），并采用统一的配置逻辑。

### **使用方法**

第一步：打开项目中的[`FlClash.js`](./Clash/FlClash.js)，获取脚本的RAW地址。

第二步：打开 FlClash，导入路径为：
```
工具 → 进阶配置 → 脚本 → 右上角“添加” → 外部获取 → 通过URL导入，粘贴下方的RAW地址 → 重命名 → 保存
```
第三步：在配置中设置覆写，点选刚刚导入的脚本。

#### **远程配置地址**

**GitHub Raw：**

```text
https://github.com/n0de-sudo/Perfect-Rules/blob/main/Clash/FlClash.js
```


## **① ⭐ Clash Mi 3.0：完美分流 + DNS 防泄漏——懒人版**

Clash Mi 用户可以使用项目提供的 `clash_mi.js`，一键导入完整的 Perfect Rules 配置。

Clash Mi 支持多平台，并采用统一的配置逻辑。
 如果希望在不同设备上使用一致的分流规则和 DNS 防泄漏方案，并且不想折腾，推荐优先使用 Clash Mi 版本。

该脚本包含：

+ 分流规则
  + 🇨🇳 国内网站直连
  + 🌍 海外网站代理
  + 🤖 AI 服务专用代理组
  + ▶️ YouTube 专用代理组
  + 🚫 广告 / 追踪拦截
  + 🏠 局域网直连
+ 🔐 DNS 防泄漏
+ 🌐 Fake-IP / DNS Hijack 等相关配置
+ 🌍 根据机场节点动态生成地区代理组

### **使用方法**

**第一步：** 打开项目中的 [`Clash_mi.js`](./Clash/Clash_mi.js)。

**第二步：** 获取脚本的 Raw 地址。

**第三步：** 打开 Clash Mi：

```
核心设置 → 覆写 → 右上角 + → 添加配置链接
```

选择 `JS` 类型，粘贴 `clash_mi.js` 的远程地址并保存。

#### **远程配置地址**

**GitHub Raw：**

```text
https://raw.githubusercontent.com/n0de-sudo/Perfect-Rules/main/Clash/Clash_mi.js
```

⚠️ **重要：**
 添加远程 JS 后，请务必将 `clash_mi.js` 的覆写方式修改为 **「内置-覆写」**，否则脚本可能无法按照预期生效。

**第四步：** 关闭并重新打开代理连接，使配置生效。

**第五步：** 在 Clash Mi 的面板中检查代理组和分流规则，根据自己的机场节点选择默认代理。

**注意：** Clash Mi 的部分版本在导入远程 JS 后，会接管部分覆写配置，这是正常现象。

------

## **② ⭐ Clash / Mihomo 完美分流 3.0**

Clash / Mihomo 用户可以使用最新的 **Perfect Rules 3.0**。

核心配置已经整理完成，你不需要自己修改，复制粘贴即可使用。如需新增规则，请提交 Issue。

### **使用方法**

**第一步：** 打开并复制 [`Clash_merge.yaml`](./Clash/Clash_merge.yaml) 的全量代码。

**第二步：** 以 Clash Verge 为例，找到订阅选项卡，双击「全局覆写扩展配置」，粘贴代码并点击保存，完美分流规则即可生效。

**第三步：** 选择你的代理节点，微调代理组即可使用。

------

## **③ ⭐ V2rayN 完美分流 2.0****（3.0 版本敬请期待）**

V2rayN 用户目前使用的是完美分流 2.0 版本。下载配置后，需要手动创建代理组和分流规则。

### **使用方法**

**第一步：** 下载项目中的 [`V2rayN.json`](./V2rayN.json) 配置文件。

**第二步：** 打开 V2rayN 👉 设置 👉 路由设置 👉 添加规则集 👉 从文件中导入规则 👉 选择刚刚下载的 `V2rayN.json` 文件。

**第三步：** 按需创建自己的专用代理组 / 专用分流规则（根据视频教程），配置好之后即可使用。

------

## **🧩 分流内容**

Perfect Rules 已经针对常见使用场景进行了分类：

+ 🇨🇳 国内网站 → **DIRECT**
+ 🌍 海外网站 → **代理**
+ 🤖 AI 服务 → **AI 专用策略**
+ ▶️ YouTube → **YouTube 专用策略**
+ 🚫 广告 / 追踪 → **REJECT**
+ 🏠 局域网 → **DIRECT**

规则会持续更新和优化。

------

## **📺 视频教程**

本项目相关配置会在 **阿尔忒弥斯实验室** YouTube 频道进行详细演示。

[**阿尔忒弥斯实验室 · Artemis Lab**](https://www.youtube.com/@ArtemisLab_Tech)

------

## **⭐ 支持项目**

如果 **Perfect Rules** 对你有帮助，欢迎给项目一个 ⭐ Star。

也欢迎提交 Issue 或 Pull Request，共同完善规则。

------

## **🔄 更新说明**

Perfect Rules 会持续维护。

主要更新内容：

+ 新增网站及服务
+ 新增 AI 域名
+ 优化分流规则
+ 修复错误分流
+ 更新 Clash / Mihomo 配置
+ 根据实际使用反馈调整规则

如果发现规则存在问题，欢迎提交 Issue。

------

## **⚠️ 免责声明**

本项目仅用于网络技术研究、学习以及配置交流。

请遵守所在地法律法规以及相关软件、网络服务的平台规则。

------

**Perfect Rules**

*Make complex routing simple.*

**阿尔忒弥斯实验室 · Artemis Lab**
