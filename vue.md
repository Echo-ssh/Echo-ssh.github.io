对于vue生命周期个人的理解

一、vue的生命周期的介绍

   每个 Vue 实例在被创建时都要经过一系列的初始化过程
   
   生命周期分为三大阶段：初始化显示、更新显示、销毁Vue实例
   
   1.初始化阶段的钩子函数：

​		beforeCreate() 实例创建前：数据和模板均未获取到

​		created() 实例创建后: 最早可访问到 data 数据，但模板未获取到

​		beforeMount() 数据挂载前：模板已获取到，但是数据未挂载到模板上。

​		mounted() 数据挂载后： 数据已挂载到模板中

   2.更新阶段的钩子函数：

​		beforeUpdate() 模板更新前：data 改变后，更新数据模板前调用

​		updated() 模板更新后：将 data 渲染到数据模板中

   3.销毁阶段的钩子函数：

​		beforeDestroy() 实例销毁前

​		destroyed() 实例销毁后

以下作为图片参考：

![微信图片_20220108115612](https://user-images.githubusercontent.com/97212804/148630682-f7dc50cc-6444-470b-8f65-24214f044223.png)

二、vue生命周期中每个钩子函数的作用
