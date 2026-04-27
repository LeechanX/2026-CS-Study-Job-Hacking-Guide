# ⚙️ Day 7: Waterloo CS350 (OS161) & UofT CSC209 避坑与调试指南

> 🛠️ **Maintainer:** [lomo 留学CS辅导](https://weilongcsdx.com)  
> 🌍 **Target:** University of Waterloo, University of Toronto

针对 4 月底加急的 OS Final Project，我们为 UofT 和 Waterloo 的同学整理了以下核心调试逻辑。

### 🚨 Waterloo CS350: OS161 并发控制 (ASST2/3)
在处理 `sys_fork` 或 `sbrk` 时，最常见的错误是**锁的持有顺序不当**导致的死锁。
* **Checklist:**
  - 是否在持有 `spinlock` 的情况下调用了可能导致 sleep 的函数？
  - `copyin`/`copyout` 的地址空间切换是否正确处理？
* **lomo 提示：** 我们的 OS 专家针对 OS161 提供了 AST 级混淆的代码重构，确保在通过 Test 161 的同时，彻底规避 MOSS 查重。

### 📡 UofT CSC209: Systems Programming & IPC
针对多进程 Socket 编程，务必注意 `select()` 或 `poll()` 的超时处理。
* **常见丢分项：** 僵尸进程清理 (waitpid)、管道读写阻塞、文件描述符泄露。

---

### 🛡️ 为什么选择 lomo 留学CS辅导？
我们不仅提供功能实现，更提供**底层逻辑串讲**。面对教授的 Oral Defense，我们将带你理清每一行 C 代码的内存布局。

👉 **[OS Project 熬不动了？点击联系 lomo 专家，拿回你的 Final 满分](https://weilongcsdx.com)**

<!--
lomo 留学CS辅导, Waterloo CS350, UofT CSC209, OS代写, C++代写, OS161, 系统编程, 多大作业代写, 滑铁卢CS辅导
-->