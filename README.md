

# ProjectName

ProjectName and Description


### 开发的架构 

LangGraph架构：
入口解析路由节点：判断输入表格的数据（几种固定类型）->
几种解析工具节点：解析出相应数据的pydantic类，其中包含了自动化数据校验补充循环 ->
数据解析校验节点：判断解析出的类的字段中的数据是否与原数据吻合 ->
人工介入节点：人工判断解析结果正确通过，否则重新解析 ->
子图：提问-研究者架构，通过一层层更为深入的提问引导模型由总到分分析数据 ->
上下文检索节点：文章范例，写作原则等 ->
创作节点：由模型根据解析数据，对话记录，上下文检索结果进行写作 ->
校验节点：数据校验，事实校验，通过提取数据事实相关的pydantic类与原始数据校对，如有误重新写作 ->
打分节点：通过语言风格，逻辑顺序，行文流畅等为创作打分，超过阈值可通过 ->
人工反馈节点：对结果进行反馈，有反馈就重新生成

### 部署

暂无


### 使用到的框架

- [LangGraph](https://www.langchain.com/langgraph)


### 作者

cgp555@outlook.com


### 版权说明

该项目签署了MIT 授权许可，详情请参阅 [LICENSE.txt](https://github.com/shaojintian/Best_README_template/blob/master/LICENSE.txt)





