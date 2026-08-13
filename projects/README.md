# projects · 实战工程

## SerialDataAcq — 队列消息处理器模板

- **来源**：桌面 `SerialDataAcq` 文件夹（2026-08-04 由 `LINE/1.lvproj` 更名，串口数据采集）
- **架构**：NI「Queued Message Handler」模板 — UI事件循环 + 消息处理循环，Enqueue/Dequeue 传递消息
- **已实现**：`VISA Configure Serial Port (Instr)` 串口配置 + 队列内持续采集（对应 CHECKLIST 阶段3）
- **远程配置**：`.aliases` 含 VI Server 远程别名 `我的电脑 = "10.100.48.150"`（远程部署用，勿删）
- **结构**：
  - `Main.vi` — 主程序（前面板 + 程序框图）
  - `controls/UI Data.ctl` — 类型定义
  - `support/` — 模板支撑 VI（Message Queue.lvlib / User Event - Stop.lvlib / 错误处理）
  - `documentation/` — NI 模板自带教程（可删除，不影响运行）

> ⏭️ 下一步里程碑：解析 STM32 端 **AA55 协议帧**（CHECKLIST 阶段3 最后一项）


## TempHumidityMonitor — 温湿度监控采集界面

- **来源**：桌面 `Labview\练习\温湿度监控`（2026-08-13）
- **用途**：采集界面制作任务——温度/湿度监控界面（智能农业上位机方向）
- **架构**：状态机类型定义 `SubVI\状态机.ctl` + 主程序 `main.vi`（含标准错误处理，LabVIEW 2025 Q1）
- **结构**：
  - `main.vi` — 主程序（前面板 + 程序框图）
  - `SubVI\状态机.ctl` — 状态机 typedef 控件
- **打开方式**：LabVIEW 2025 Q1 直接打开 `main.vi`（独立 VI，暂未建 .lvproj）
- **命名说明**：工程目录英文命名 `TempHumidityMonitor`（遵循仓库英文命名规则）；VI/ctl 内部文件名保持原样，避免破坏 VI 引用关系
