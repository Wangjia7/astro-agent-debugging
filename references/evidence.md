# 证据来源与覆盖边界

整理日期：2026-10-14。项目显示名及实际目录使用“天文agnet”；用户称“天文agent”。原项目根目录为 `/Users/jqwang/Documents/ChatGPT/天文agnet`。下表均为相对该根目录的路径。

本次发现 4,208 个候选 Markdown/报告/状态等路径，对不超过 300 KB 的 Markdown 按内容去重形成 328 份文档索引。索引代表发现范围，不代表逐行复核了所有文件。重点阅读下列审计、验证报告、研究记录及 CURRENT，结合其余材料检索归纳。历史报告所述测试结果是历史证据，本次没有重跑科学矩阵、远程 API 或已清理的大日志。

案例中的“已证实”指对应历史报告明确复现或验证；“失败假设”指候选未通过其预定门禁，不等同实现错误；“边界”表示记录不足以支持更强结论。CURRENT 是状态指针，以其引用的源码和产物身份判断适用版本。历史问题可能已经修复。

哈希固定本次读取的文档字节，不能单凭文档哈希证明其中引用的实验确实可复现。移机后可以靠相对路径和哈希在已授权的备份中查找；技能正文与案例本身可独立使用。完整发现目录见 [corpus-index.tsv](corpus-index.tsv)。

## 重点来源

### E01 — 协议边界、字段/时长搜索、异常分类、软预算、旧测试

路径：`outputs/agentic-review-v01/REVIEW.md`  
SHA-256：`4c8af4b2f22f9eb8a23784570fbf593113bee8e89d73617cd889c0f8299a63fb`

### E02 — 评分口径、独立曝光、不可达上界、缺初始化

路径：`outputs/science-audit-v1/REPORT.md`  
SHA-256：`d0f477ce58bb5dfc3cecbbf06254302a5c4b71071051c0f3fc9f33daf020f22a`

### E03 — 物理尺度、故障识别、工程文本、时区、日志与分母

路径：`outputs/gosim-v34-feedback-analysis.md`  
SHA-256：`c1acb3c9e07de036af5be97c915a291694254d373852b5e4f9014cea29522e51`

### E04 — 共享成本、请求窗口、runtime guard、native 构建身份

路径：`outputs/gosim-runtime-v3.6-validation.md`  
SHA-256：`e56b56f400b1c4a5ebb87fceaed41fc8f1e023db9da1bd7aea80ba2084457d1f`

### E05 — QA、重复消息、失效重算、独立账本和终末反馈

路径：`outputs/gosim-inspection-v3.5-validation.md`  
SHA-256：`fcbd4fcc3718df2872242bdcda1a82d0d2ec11fbf96eafc260eeb74b00e77a22`

### E06 — 状态顺序、实例配置、月亮历元、天气过滤

路径：`outputs/gosim-fusion-v3.3-comparison.md`  
SHA-256：`332de871303ff69e48c6e340fc13bb3d83d2019537a224850031c71cc89b23f0`

### E07 — CPU 低计、不可见目标、天气与故障混淆

路径：`outputs/gosim-pro-normal-v3.2-validation.md`  
SHA-256：`50e9384cc3c9b8c8792f863a428153e2a9f1116c72490a719ba467e13120dd0a`

### E08 — 保留环境前缀、CPU 档位、搜索放宽反例

路径：`outputs/gosim-logcpu-v3.4-validation.md`  
SHA-256：`08eac0832615824f1b6ae3902b906f6a395d2ebdf5af19486cf3285db4f5477e`

### E09 — 终末反馈消费时序与回放污染

路径：`work/observer-order-mean/independent-final-review.md`  
SHA-256：`e76db91fff25c4e2eeadd9ff2ac58d827c3a891e0966d10e25b7648c1e0f8af6`

### E10 — planned 失败、seed=null、输出目录冲突、事后登记

路径：`work/observer-order-mean/evidence/registration-chronology.md`  
SHA-256：`9437cacd97573ab864b9db9e48bc6014b56823c705c3ac7a059f837f661cc44f`

### E11 — 有限预算、失败候选、API 传输、实际执行与验收

路径：`work/observer-v111/CURRENT.md`  
SHA-256：`ff14a28397854a62b0439ee2f7c346fa128801d8da4a5078eecedebc35cfa46e`

### E12 — 冷/热缓存和整路径功能门禁

路径：`work/observer-sky-exact-cache/FINAL_REPORT.md`  
SHA-256：`4e5dc0a747e62e53162b775afc21e01b5646c4da90077155bfdad54f86e96fb7`

### E13 — 嵌套计时与成本假设被否定

路径：`work/observer-rollout-cost-audit/CURRENT.md`  
SHA-256：`8675d43f925c7abc71156ac08a3b9d4dc8004554349aa7d06ab0a31568bcbe5c`

### E14 — 旧校验器、消融开关被覆盖、wrapper 假网络错误

路径：`work/observer-v0253/deliverables/更新与测试报告.md`  
SHA-256：`16efd1d6133c6e3ec6974e9242116e510de52b340b830845d146f32e4971fc53`

### E15 — API cadence 提前消耗应急额度

路径：`work/observer-v0262-long-validation/CURRENT.md`  
SHA-256：`81fc7c8b9574fafbf1168014280e8ec00dde8e72ecbf08453b8f7f765877d111`

### E16 — 数值收益与 REQ 门禁冲突

路径：`work/observer-v0262-final/CURRENT.md`  
SHA-256：`66ede2b26c5a52473130b4ef5f535b181616398cd0c89d6b878497f484a7c824`

### E17 — 计算完成但验收失败、inconclusive、双角色与零安装

路径：`work/observer-v100/CURRENT.md`  
SHA-256：`a9f41f27c71603090d47d2a4b861900ac97ec3202f2a9f4e0574aa2a79e8474c`

### E18 — 配对 ON/OFF 结果与不完整基线

路径：`work/observer-v101/CURRENT.md`  
SHA-256：`e978ed557c6a0cbabcf1f2e11c9526e5ae26eeae64517af8e78c21ee9cbda974`

### E19 — manifest 二维数组与最终源码证据范围

路径：`work/observer-v200/manifestfix-delivery/source/CURRENT.md`  
SHA-256：`333bb5ceee371200468ec154b3a8772952c35041b2aa12bb2b2e4d493f89bd37`

### E20 — JSONL、cwd、ABI、云端失败根因边界

路径：`work/observer-interface-v110/v1.1.0-接口检查说明.md`  
SHA-256：`c195bb207b25154b27020e606f1847985ffe344bcca981cb8f633dfdd897281e`

### E21 — 全局/局部编号、区域映射、输入版本与缺失连接

路径：`work/desidr3_v2_audit/numbering_from_fortran.md`  
SHA-256：`b21311ee0d4da8ca14e4fd7d7630640231be55d1c4d463b5135fb63ef80dedf5`

### E22 — 超时剔除、母 seed 派生卡与开发/验证选型

路径：`work/observer-version-v025/experiments/router-study-v03/report.md`  
SHA-256：`92ddc8b5d76f8a4751fc90e423d0e4fc1578332a0905f31bb3ac72062918484b`

### E23 — 中点候选假设、样本身份与预算外特征成本

路径：`work/observer-version-v025/experiments/midpoint-study-v06/final-report.md`  
SHA-256：`63f04b1e49a5f3a8a208ef165aeea240d2fcdfe435cc04af56433c7af062e02d`

### E24 — 并发混杂、有限轨迹等价、CPU 与科学收益

路径：`work/observer-version-v025/experiments/cpp-pilot-v07/report.md`  
SHA-256：`17c970ab56f6ab6982275e8aadf44e0cdc66af4132569c9006f04147d10d0bd6`

### E25 — native 顺序、数值与物理不变量

路径：`work/skill-extreme-optimization-v12/saved-version/observer-policy-router/references/extreme-code-optimization.md`  
SHA-256：`714e94848d4760df2894f7b11d57482616b7f222edee5ab820cf6713d8fbc727`

### E26 — 预测 MSE 改善但整季 REQ 退步

路径：`work/observer-frame-agent/研究记录.md`  
SHA-256：`55c600531b71ff69459e49363c6b9f014728eaa66c9f47b5df9d04fd465d86ab`

### E27 — 均值上涨但单卡 REQ 失败、API 归因与留出污染

路径：`work/observer-feedback-order/complete-matrix-report.md`  
SHA-256：`290bb04adc5ca2884f3beda5c31cce11db883eeba69a4425cc99d076d66a22f3`

### E28 — 连续窗口与真实候选链

路径：`work/observer-depth-windows/PLANNER.md`  
SHA-256：`d8641b944d0a1913c2376f83315a36ff6b82ad75ab1184f0c5f7aeed93681d2c`

### E29 — 候选排名/精算入口瓶颈

路径：`work/observer-required-entry/CURRENT.md`  
SHA-256：`1dad8f92fb3ca5fcc1afde0e47e1979a0b96505bca943c8950a96d6a10e07be9`

### E30 — 不变量与未触发分支覆盖

路径：`work/observer-objective-consistency/independent-review.md`  
SHA-256：`a9bc75d590ca94a05fdb05c37876643cfd1ef7b4d0c2d708ea8118db65fa3ba6`

### E31 — 不可达上界不能直接当成可恢复收益

路径：`work/observer-science-loss/CURRENT.md`  
SHA-256：`09d3cfd478aa5e29b4ee460de94a0c7255efa931ce38bfb26065e0b2fa3d49fc`

### E32 — 科学分上涨但义务门禁失败

路径：`work/observer-full-obligation/independent-review.md`  
SHA-256：`f53d725b724a01da2406448b866db21c2946ac7e60d223fb23e1ecd0b929f39e`

### E33 — 逐卡与均分验收、缺同源 OFF 的因果限制

路径：`work/observer-v111-score-validation/FINAL_REPORT.md`  
SHA-256：`ebcc8edb4591154ab8bd3dacbaeab828bca645ad869351a7a9aae2b5b4c7c763`

### E34 — 完整矩阵、失败门禁与真实 API 角色

路径：`work/observer-v111-continuity-validation/FINAL_REPORT.md`  
SHA-256：`cf8de33be62746140d09557d1e16f57717e95e39371323246add49f46278f1aa`

### E35 — 测试修复与机制未触发

路径：`work/observer-critical/研究记录.md`  
SHA-256：`de9fdc13657f870085692d09ca5da30e79abb50651f0ec2818f8deee533f9426`

### E36 — 选择标签、识别区间与泛化边界

路径：`work/observer-depth-calibration/independent-review.md`  
SHA-256：`dbd4d9d5539be89f860794be7fb4fa750ccb42680ca445f9c70d00e7719a6ec1`

### E37 — 固定终点 shadow 与整季因果差异

路径：`work/observer-first-depth/CURRENT.md`  
SHA-256：`373e2ac482df566cbfc7de4994c75868aba298353c8bf430e0bb5797f349187d`

## 会话归档操作来源

O01–O04 来自本次上传/清理会话，属于操作流程教训，不能归入科学算法缺陷。回执只能证明其中记载的文件与校验层级；Python 能力和断线等过程错误来自会话工具记录。回执相对本次工作目录：

- `outputs/starter-migration-receipt.json`、`outputs/starter-migration-manifest.json.gz`。
- `outputs/astro-migration-receipt.json`、`outputs/astro-migration-manifest.json.gz`。

用户已选择“上传去除密钥的版本，敏感配置单独留在本机”。本 skill 不包含密钥、配置原文或敏感备份。

恢复入口：[starter 归档](https://github.com/Wangjia7/Gosim_v72/releases/tag/starter-documents-backup-2026-10-13)、[项目归档](https://github.com/Wangjia7/Gosim_v72/releases/tag/astro-project-backup-2026-10-13)。本次整理没有重新下载这些分卷。此前本地完整恢复校验和 GitHub 服务端摘要校验通过；完整远程重新下载未完成。不要把两种校验表述为已做完整远程恢复。
