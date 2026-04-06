# workflow_devmate 设计模式与实践手册

## GoF 23 模式分组

### 创建型
- Singleton
- Factory Method
- Abstract Factory
- Builder
- Prototype

### 结构型
- Adapter
- Bridge
- Composite
- Decorator
- Facade
- Flyweight
- Proxy

### 行为型
- Chain of Responsibility
- Command
- Interpreter
- Iterator
- Mediator
- Memento
- Observer
- State
- Strategy
- Template Method
- Visitor

## 当前项目优先模式
- Strategy：
  - 用于不同执行/回退/失败治理策略切换
- State：
  - 用于任务状态、schedule trigger 状态、角色创建阶段
- Facade：
  - 用于对外暴露稳定 service 入口
- Adapter：
  - 用于 DB、文件态、运行态三种真相源之间的桥接
- Template Method：
  - 用于 smoke / 验收 / 质量巡检步骤统一
- Observer：
  - 用于事件流、状态更新、看板刷新

## 何时优先重构
- 文件超出行数门槛
- 同一逻辑同时出现在 `DB + 文件 + API + 前端`
- 同类异常被重复修 2 次以上
- 热修已开始侵蚀长期结构
