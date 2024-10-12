# Fx
Clean architecture

## 清晰的架构分层

> src/
>> Core/                # 核心业务逻辑（Entities, Aggregates, Interfaces）
>>> Entities/           # 领域实体（User, Role等）
>>> Interfaces/        # 核心接口，如仓储接口 (IUserRepository)

>> Application/         # 应用层逻辑（DTOs, Services, Use Cases）
>>> Services/          # 业务逻辑服务
>>>UseCases/          # 用例（处理业务逻辑）

>> Infrastructure/      # 基础设施层（实现领域接口，第三方服务集成）
>>> Identity/          # Identity相关代码，数据库上下文，Identity配置
>>> Repositories/      # 实现领域仓储接口的具体类

>> WebAPI/              # Web层（控制器，API接口）
>>> Controllers/       # API控制器（处理HTTP请求）
>>> Dtos/              # 数据传输对象（前端与后端交互的数据对象）
