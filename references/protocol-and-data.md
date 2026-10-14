# 协议、数据、交付与归档

历史案例：P01–P08、D01–D02、O01–O04。

## 官方合同与最终包

从 initialize 读 min/max duration、光纤/目标范围和版本。正常、闭站、无候选、夜末、回退使用同一合法动作入口；把实际 process 输出交官方 normalize 验证，自写 validator 不是最终判据。

协议支持 until_utc 时，使用严格未来且保留必要精度的时刻表达越界 duration 等待；按合同互斥字段。官方 runner 展开等待并投递期间消息，不自行跳过潜在请求。

声明的传输别名与实际 participant protocol 分开；canonical 推荐不证明旧别名是失败根因。云端准备错误需要该次 build/launch 证据，本地同名卡不能代替。

stdout 仅 JSONL，安全诊断进 stderr，异常非零退出。覆盖不同 cwd、EOF、非法输入、缺资源、坏 native/ABI 及 fallback。

从最终冻结源打包，新目录解包后官方 parser → manifest build → manifest run → JSONL/结束。直接 Python 启动不能覆盖二维 run 数组、相对路径、缺资源或 ABI。

部署系统重建 native；macOS .so 不冒充 Linux。漏构建而走 Python fallback 的评分单独登记，不能和 native 基线冒充等价。核对当前保留 env 前缀及开关实际消费者，不从旧前缀案例或名字推断现行规则。

比赛包与证据包分开；按规则排除密钥/.env、truth、卡片、宿主二进制。mock、native、真实 API、Linux、网站分别给状态。

## 科研编号与缺失

沿生成源码区分全局 ID、筛选内部序号、输出行号和区域映射；目录 NGC 名称不决定实际运行区域。明确整数宽度与唯一性。

全局 ID 精确 join，缺失位置 -1 先拦截；区域 1-based index 先经对应 galaxyID 向量再 join。仅在证明 ID 连续时使用 ID-1。

旧输出与当前筛选不一致时核对源、输入、规则、float 类型、文件身份，不能仅给缓存编号减一而保留错属性。按输出精度预定容差，报告缺失，不宣称重建尚未取得的全量服务器数据。Notebook 说明进 Markdown cell；语法通过不是科研验收。

## 备份清理分支

仅任务包含上传/清理时启用；本 skill 不授权外传、发消息或删除。

定位真实路径、来源清单、目标可见性及删除范围。权限、网络、上传能力分别核验。密钥检查覆盖配置、日志、嵌套 ZIP 和 Git 历史；按用户选择单独保留/加密，不能隐含公开。

按当前限制选分卷/附件，保存路径、mode、链接、空目录、size、SHA-256。批量前探测解释器能力，不假定 file_digest、SpooledTemporaryFile.seekable 或 tar 流 compresslevel 可用；可复用部分先确认不可变身份。

区分原件、脱敏件、分卷和敏感副本 hash。恢复验证包含目录/链接集合、内容和敏感覆盖；说明与格式一致。

平台独立 checksum/size、下载 checksum、完整恢复是不同层，分别报告。有限重试/续传核对 Content-Range 和长度；部分下载不冒充完整。网络失败不写成已下载通过。

删除前复核当前原件身份，严格按授权范围。大文件清理按已说明门槛，仅删对应文件并保留其余目录/Git；某次 10 MiB 不是通用默认。清理临时副本并输出清单、敏感副本位置及未完成验证。
