Data Center Artificial Intelligence (DCAI) 旨在通过 AI 技术赋能数据中心业务

简介
当前 DCAI 涵盖 AI-OPS 和 AI-Cooling 两部分

AI-OPS
开发与部署
开发环境（Python 解释器与虚拟环境及其依赖安装）link
项目部署 link
AI 功能与接口
AI-OPS
动态基线 AI 接口 link
如何回测 link
后续工作
根据当前 AI 已开发的接口，后端进行评估，给一些建议和需要优化内容，我能想到的有如下：

@产品 哪些参数需要对外开放，暴露在产品前端（需要和产品一起讨论）
@产品 确定试点机房与首批测点，用于真实场景的回测
@后端 基于产品确定的试点机房，给到数据
@后端 数据流转细节沟通，输入输出数据的时间长度、采样频率、格式，后续变更扩展性等
@后端 dcai 项目的结构：项目包含后端和AI，结构上怎么做更好的隔离
@后端 dcai 环境依赖与部署使用技术栈选型 (pyenv + poetry) 讨论
@后端 AI 接口返回值的形式需不需要优化
@后端 联调与镜像文件（需要前置步骤完成）
@算法 模型细节优化、文档完善、增添单元测试
AI-Cooling
后续工作
@算法 调研学习AI-Cooling方案，设计产出GLP方案
基于GLP-IDC真实数据定位到当前人工调优的可优化点
基于可优化点设计方案：模型选型、业务评价指标、回测体系等
@算法 将 aiops 与 aicooling 项目分开，方便后续的部署、迭代升级