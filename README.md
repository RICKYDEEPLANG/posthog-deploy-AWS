基本信息
- 服务器:AWS EC2 ip-172-31-34-171
- 域名:https://posthog.neodrop.ai/
- 监控:http://54.69.200.172:3000/
- mcp:https://deeplang.feishu.cn/wiki/XaSSwuj5WieduukNz71cJjUonKc
运行版本(两层)
容器里实际跑的代码 = 镜像提供运行环境/依赖 + 挂载的源码覆盖应用代码,所以版本分两层看:
① 镜像层
- 基于上游 commit ee1d1843b7d31d77592a9bc128c0f70520d6c931 构建
- 其余全部镜像(posthog-node、ghcr 微服务、基础设施、监控)的 digest 见 IMAGES.md
② 挂载的源码层(应用代码以这层为准)
- 分支:origin/fix/count-tokens-api-fallback
自有改动(通过挂载生效)
暂时无法在飞书文档外展示此内容
源码已推送到 origin/fix/count-tokens-api-fallback,远端有备份。

