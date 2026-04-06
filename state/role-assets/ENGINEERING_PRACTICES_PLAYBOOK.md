# workflow_devmate 工程实践手册

## 默认实践
- 先拉最新代码再开发
- 小批量改动，小批量验证，小批量推送
- 运行态不作为开发面
- 线上热修必须回放
- 先证明问题，再给方案，再改代码

## 当前项目强约束
- `workflow_code` 是唯一代码根仓
- `.repository/<developer_id>` 是唯一开发面
- `.running/*` 只做运行与部署
- 所有修改先验证，再推回代码根仓

## 当前项目优先技术债
- schedule 中文编码
- schedule / assignment / dashboard 真相源一致性
- 24h 连续运行稳定性
- smoke baseline 可稳定调用
- 页面状态看板与真实任务状态一致
