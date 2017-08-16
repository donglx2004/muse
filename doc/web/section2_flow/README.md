执行流水
======

        执行流水会显示所有已经执行的任务的执行情况，是以执行为维度，每一次执行为一条执行记录。


## 查询条件
* 调度日期:某次执行计划调度的日期
* 执行日期:真正执行的日期
* 执行开始日期>=:开始执行的日期
* 执行结束日期<:最后执行的日期
* 任务ID:任务ID，模糊获取可选的id列表，再选择对应的任务ID，支持多选
* 任务名称:根据输入模糊获取可选的任务列表，再选择对应任务，支持多选
* 任务类型:选择任务的类型(Hive、Shell、Java、MapReduce、Dummy)，支持多选
* 执行用户:触发执行的用户，支持多选
* 状态:执行的状态，支持多选

## 状态
* 等待:任务还在等待其他执行条件满足，比如前置任务未执行
* 准备:任务已经满足触发条件，在队列中等待调度
* 运行:任务正在执行
* 成功:执行成功
* 失败:执行失败
* 终止:任务被强制停止
* 删除:任务被删除

## 执行列表
* 默认显示执行ID、任务ID、任务名、任务类型、执行用户、调度时间、开始执行时间、执行结束时间、执行时长、状态、操作。
* 操作列可以点击查看任务依赖、当前执行详情、重试记录，并且可以原地重跑或删除任务。
* 点击任务名可以查看任务的详细配置信息