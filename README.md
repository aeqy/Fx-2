# Fx
Clean architecture

## 清晰的架构分层
   
`清晰的分层和职责分离至关重要。Clean Architecture 的基本原则
（例如，内核层与外部依赖的解耦）依然适用，但具体的实现需要更加严格的规范化。`



### 分层结构：

#### 项目结构：展示分层结构和依赖关系。
##### 领域层（Domain Layer）：定义核心业务逻辑和实体。
##### 应用层（Application Layer）：定义用例和服务。
##### 基础设施层（Infrastructure Layer）：配置 OpenIddict 和实现身份验证逻辑。
##### 接口层（Presentation Layer）：处理用户请求。