
# 系统框架结构的规范
=================================================================

1、静态页面中需包含两部分：
	1. #FrontLoading 层，该层旨在页面真实模板渲染完成前显示 loading 状态，在页面完成渲染后需 hide 或 remove
	2. .body 层，该层用于填充真实模板数据，建议在该div上添加当前页面的一个私有变量名A，
	    页面中的私有布局样式均写在A的命名空间下，防止样式冲突，变量名污染
--------------------------------------------------------------------------------------------------------------------- 

顶部固定导航栏	div.inner-header 
页面正文		div.inner-body
底部固定		div.inner-footer

