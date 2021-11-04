# awesome-lowcode

> A low-code development platform (LCDP) is software that provides an environment programmers use to create application software through graphical user interfaces and configuration instead of traditional computer programming.


- 全程可视化设计

  可视化的界面编辑器，通过面向业务的界面设计能力为传统开发者以及其他的应用参与者提供服务。

- 低代码编写能力

  平台必须提供应用在各层次、各阶段快速进行代码干预和插入的能力，比如添加自定义组件、定制个性化逻辑处理、信息流传过程中三方应用嵌入等场景。

- 全软件生命周期管理([aPaaS](https://zhuanlan.zhihu.com/p/69177511))

  从应用开发构建，到发布后的运维、运营，再到应用产品升级，形成了全生命周期管理。会涉及到产品经理、需求分析师、架构师、开发人员、测试人员、运维人员、运营人员、技术支持人员等等各种各样的角色本身工作和协作工作，低代码开发平台必须要具备全生命周期特性，才能真正达到从整体把控应用开发全过程实现快速交付、降低开发成本的目标。


## 核心功能
- UI Builder
- Form Builder
- Flow Builder
- Table Builder
- BI Report Builder

## 国内外低代码平台
- 微软PowerApps https://powerapps.microsoft.com/zh-cn/
- 谷歌的Appsheet
- AWS 的Honeycode
- 轻流 https://qingflow.com/
- 阿里宜搭 https://www.aliwork.com/
- 西门子Mendix https://www.mendix.com/zh/ 
- 明道云
- 简道云
- BuildRun https://gobuildrun.com/zh/
- 奥哲-云枢 https://ldpage.cloudpivot.authine.com

## 使用案例
- [3个小时，从学到做，我用低代码平台搭了一套管理系统](http://www.woshipm.com/pd/4382199.html)

## 技术方案
- 表单驱动
- 模型驱动

1. 前端可视化技术方案 
	- 动态表单生成技术
    - [formio.js](https://github.com/formio/formio.js) - 比较复杂，配置项繁多
    - [react-interactive-dynamic-form-generator](https://www.npmjs.com/package/react-interactive-dynamic-form-generator)
  	- [Element UI Form Generator](https://github.com/JakHuang/form-generator)
  	- [Alibaba formily-editor](https://github.com/alibaba/formily-editor)
  - 可视化界面编辑
    - [H5-Dooring](https://github.com/MrXujiang/h5-Dooring) 
    - [vvvebjs](http://www.vvveb.com/vvvebjs/editor.html)
    - [form-generator](https://github.com/JakHuang/form-generator)
    - [avue-form-design](https://github.com/sscfaith/avue-form-design)
    - [vue-ele-from](https://github.com/dream2023/vue-ele-form)
    - [vue-form-making](https://github.com/GavinZhuLei/vue-form-making)
    - [f-render](https://github.com/dream2023/f-render)
    - [form-js](https://github.com/bpmn-io/form-js)
2. 前端组件化
3. 多租户方案
   1. 数据如何存放？
   2. 私有化部署？
4. 前后端模型关联
5. 流程编辑器 
   - [字节开源的可视化流程编辑器](https://github.com/bytedance/flow-builder)
   - [LogicFlow](https://github.com/didi/LogicFlow)
   - [vue-flowchart-editor](https://github.com/jnoodle/vue-flowchart-editor#readme)
   - [easy-flow](https://github.com/BiaoChengLiu/easy-flow)
   - [workflow-ui](https://github.com/go-workflow/workflow-ui) - 仿宜搭Vue
   - [workflow-react](https://github.com/cedrusweng/workflow-react) 钉钉审批配置-react版
   - [Workflow](https://github.com/StavinLi/Workflow)  钉钉审批配置-vue版

6. 数据模型编辑
7. 自定义报表


```
数据结构设计
插件体系设计
多数据源支持
页面模版支持
UIUX
```

### 数据结构

(*一个应用一个大的JSON Schema配置文件?*)

用户 > 应用 > 标签（菜单) > Page(组件*) > 列表 > 报表

- Page
  - Metadata
  - Schema
  - Components
  
- Component
  - Schema
    - Form
  - Data
    - ComponentRecord
  - Binding ( DataSource - Component Data )

- DataSource
  - Resources (REST)
  - Metadata
  - ACL



```
- 前端表单如何与后端数据绑定？
- 多租户?
```

### 可视化页面组件

前端部分的可视化组件

- [Moveable](https://github.com/daybrush/moveable)
- [百度AMIS](https://baidu.gitee.io/amis/zh-CN/docs/index)
- [Flow-Based Programming for JavaScript](https://noflojs.org/)


## 技术选型
 - 前端
   - React (Next.js)
   - Angular
   - Vue (Element UI)
 - 后端
   - Spring Cloud体系
   - Redis
   - MongoDB

## Reading
- [低代码平台和社区开发者的崛起：更多解决方案还是更多问题？](https://www.infoq.cn/article/0PrNu154Zbjrip5u2BgI)
- [ZooTeam 拍了拍你，来看看如何设计动态化表单](https://www.infoq.cn/article/Ndi3VUgJ5ydhdMXfAXQ5)
- [[译]如何优雅地用 Vue 创建数据驱动的用户界面 ](https://juejin.cn/post/6844903616189300744)
- [页面可视化搭建工具技术要点](https://github.com/CntChen/cntchen.github.io/issues/17)
- [页面可视化搭建工具前生今世](https://github.com/CntChen/cntchen.github.io/issues/15)
- [宜搭产品成长之路](https://zhuanlan.zhihu.com/p/78015287)
- [20+个可视化搭建工具，一次玩个够](https://my.oschina.net/u/4585038/blog/4760011)
- [从低代码到无代码：可视化逻辑编排](https://mp.weixin.qq.com/s/LL8rZl-Ee8HYOs3375usVA)
- [无代码编程](https://www.phodal.com/blog/low-code-programming/)

## Sandbox


## Awesome awesome-lowcode
[awesome-lowcode](https://github.com/taowen/awesome-lowcode)
[awesome-lesscode](https://github.com/dream2023/awesome-lesscode)

