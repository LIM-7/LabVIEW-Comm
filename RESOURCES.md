# LabVIEW 通信学习 · 配套资源

## 📖 核心参考书
- **《LabVIEW通信程序设计》**（人民邮电出版社，ISBN 978-7-115-60196-4）
  - 知网在线阅读链接：由用户提供（`kns.cnki.net/reader/flowpdf?...`）
  - ⚠️ 书中"通信"章节目录待对照——打开书后，把目录发给 Claude，可补进 LEARNING_PLAN.md 的对应阶段

## 🔧 软件
| 资源 | 用途 | 备注 |
|---|---|---|
| **LabVIEW Community版** | 编程环境 | NI官网免费注册下载，约4-5GB，**装到E盘** |
| **VSPD / Virtual Serial Port** | 虚拟串口对 | 无硬件时在本机测试串口，模拟COM1↔COM2 |
| **虚拟仪器驱动** | VISA | 安装LabVIEW时勾选 NI-VISA，串口通信必需 |
| **串口调试助手** | 参考/对照 | 可先用现成助手，理解后再自己写 |

## 📚 延伸资料
- **NI 官方教程**：`learn.ni.com` 有大量中文入门教程
- **LabVIEW 帮助**：软件内置（按 Ctrl+H 即时帮助 / 快捷键打开 Context Help）
- **社区论坛**：`forums.ni.com`、`bbs.elecfans.com`（电子发烧友）

## 🔗 与你项目的结合点
- 你的 **STM32 智能农业**协议帧：`AA55 cmd len data checksum(~sum)`
  - 学完阶段2/3后，就能用 LabVIEW 解析这一帧 → 显示温/湿/光照/土壤
- 你之前规划的**远程报警上位机**（温度>30、湿度>75、光照<50、土壤<30）→ 就是 LEARNING_PLAN 阶段6的实战项目
