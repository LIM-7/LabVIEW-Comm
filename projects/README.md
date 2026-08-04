# projects · 实战工程

## LINE — 串口采集演示（队列消息处理器模板）

- **来源**：桌面 `LINE` 文件夹（原 `1.lvproj` 工程）
- **架构**：NI「Queued Message Handler」模板 — UI事件循环 + 消息处理循环，Enqueue/Dequeue 传递消息
- **已实现**：`VISA Configure Serial Port (Instr)` 串口配置 + 队列内持续采集（对应 CHECKLIST 阶段3）
- **结构**：
  - `Main.vi` — 主程序（前面板 + 程序框图）
  - `controls/UI Data.ctl` — 类型定义
  - `support/` — 模板支撑 VI（Message Queue.lvlib / User Event - Stop.lvlib / 错误处理）
  - `documentation/` — NI 模板自带教程（可删除，不影响运行）

> ⏭️ 下一步里程碑：解析 STM32 端 **AA55 协议帧**（CHECKLIST 阶段3 最后一项）
