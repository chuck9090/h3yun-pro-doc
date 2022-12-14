# 前端常用实例

## $.SmartForm.ResponseContext

```$.SmartForm.ResponseContext``` 仅在表单前端代码中可用，可以通过此实例属性获取表单的当前状态。

### 属性

| **属性名**            | **数据类型** | **说明**                                                       | **示例** |
|--------------------|----------|--------------------------------------------------------------|--------|
| ActivityCode       |          | 流程节点编码                                                       |        |
| DisplayName        |          | 表单名称                                                         |        |
| FormDataType       |          | 表单数据类型                                                       |        |
| FormMode           |          |  表单模式，0为审批/办理 ，1为办理完结 ，2为创建 ，4为查阅                        |        |
| InstanceId         |          | 当前表单数据的流程实例                                            |        |
| IsCreateMode       |          | 是否创建模式，true：创建模式                                       |        |
| BizObjectId        |          | 当前对象ID                                                       |        |
| BizObjectStatus    |          | 当前对象状态，取值及释义：0 草稿；1 生效/流程结束；2 流程进行中；3 作废|        |
| SchemaCode         |          | 当前表单的SchemaCode                                                 |        |
| IsMobile           |          | 是否移动端，true：移动端                                           |        |
| Originator         |          | 发起人用户ID                                                      |        |
| OriginatorCode     |          | 发起人用户名                                                       |        |
| OriginatorParentId |          | 发起人所在部门ID                                                    |        |

### 示例

1. 在表单打开时，判断是否是通过列表上的新增按钮点开的（即新增模式）：

2. 在表单打开时，判断是否是通过列表页数据标题点开的（即表单数据查阅模式）：

3. 在点击 提交/同意 按钮时，判断当前流程节点：


## this

```this``` 仅在表单前端代码的事件中可用，可以通过此实例属性获取表单的控件实例，用以操控控件。

!> 建议：事件内第一句代码，用一个变量转存 ```this```，以防指向错误的BUG。

正确指向与错误指向示例：

