# 预算、模型流程与实验判断

历史案例：B01–B08、A01–A07、E01–E09。

## 计量与 runtime guard

区分 process/子进程/线程/native CPU、标准化 CPU、agent/engine/runner wall，写出当前标定换算方向。旧 macOS 曾约 41.7 倍低计，该倍数不是通用修正常数。

用有界忙循环和实际等待探测计费，覆盖 native/子进程。引擎和模型等待是否计费依当前合同；本机可信 hook 不修改评分规则，不代替线上 cgroup 验证。

记录实际采用档位的成本。曝光、响应和平台自动 waits 分开；嵌套 timers 说明包含关系，不直接求和。projection 用当前真实单位更新。

deadline 覆盖初始化、扫描、打包、native、全积分、counterfactual、日志及最终选择，不只某循环。保留合法 incumbent；资源不足回退已验证方案。实时余量扣前阶段成本、基础后续计划和安全余量后才准入验证。

分片前瞻需足够完成最小比较；未完成输出 inconclusive，缺失收益不是零。声明额度身份与 remaining 分开，检测缩额不能由人为 floor 掩盖。固定档位和 infinity deadline 不能绕过 runtime guard。

CPU 加速会影响自适应动作。同状态固定工作差分与同预算整季分开。native 等价加速保留迭代/tie/求和顺序、v>0、边界 fallback、数组生命周期及 ABI；裁剪/重排候选是策略改动。

先测真实瓶颈和功能门禁。冷缓存快、热缓存慢、profiling wrapper 开销和仍只完成 2/6 验证路径不能宣称端到端改善。

## API 四层证据

安全错误类别区分 DNS/权限/网络、HTTP、finish_reason、外层 JSON、工具参数、schema、数值 gate 与 budget inconclusive，记录阶段和长度，不打印密钥或敏感原文。一串 ValueError 不能定位模型能力。

分别计数 attempts、provider replies、proposal/review、有效角色、完整数值验证、配额安装和实际动作变化。mock 验 schema，真实回复验接口，进入计划验执行，同源 OFF/ON 验综合效果。

沙箱 DNS 失败是传输失败；真实 API 沿用授权，失败尝试/冒烟/取消都入账。skill 不授予新的外部调用。

调用 cadence 从当前用户要求读取；初始、checkpoint、异常准入与上限独立测试。修 cadence 与修数值策略分别冻结。retain 不必启动 forecast，inconclusive 不伪装通过。

OFF/ON 差异可能混合等待、验证 CPU、host load、降档及建议内容。找真实安装及首个物理动作分歧后再作窄归因；0 install 仍可能有时间开销，不能称 API 完全无影响或提分。

## 身份、登记与验收

按任务规模预先固定假设、父源、输入/评分器/配置/RNG、对照、单位、预算、终止和验收条件。轻微修补不自动需要大矩阵；使用登记器时 planned 成功回执是正式入口。

确定性 seed=null，随机试验记录真实 RNG。核对返回码、登记读回、输出隔离、运行文件哈希再启动。技术失败消耗预算，修复用子版本；事后补记注明 retrospective，不补造时间。

源、runtime copy、native、flags、提示和包分别冻结。测试过旧接口或 fixture 缺失时修测试入口，不改生产配合旧测试、不放宽容差。源改变后，数值/计费/真实 API 的最终成绩来自最终源。

完整有效季才有 eligible score；超时/错误/中断分别保存，null 不补成部分成绩。计算 completed 与科学 accepted 是两条轴。

逐项解释当前门禁：REQ 若不增，science/均分上涨也不能覆盖。每卡+10%、均分+10%、D 不退步、双 API 角色按合同分别报告，不事后换门槛。

基线分母须完整有效、配对及身份确定；不能借修复前成绩作最终源成绩。固定正常控制及计费，不同并发/标定时间差不直接算加速比。

留出用于选型/定位后转开发数据。母 seed 的派生纬度/周期/密度不是独立环境数；开发集选赢家，验证同一策略，不能验证集重选赢家。

## 停止方向

- 技术失败修契约，不作科学反证。
- inconclusive 先测完成路径成本及最小准入，不默认加预算。
- 机制未过查入口/精算/保护/质量断点，关闭无依据整季扩展。
- 完整验收失败保留不利卡/REQ/接口，转向一个有新证据的假设。
- 新任务可设新预算/新留出，但不改历史失败为通过。
