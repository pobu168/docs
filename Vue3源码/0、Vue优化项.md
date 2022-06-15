##### 源码优化

1、更好的代码管理方式：monorepo

2、有类型的JavaScript:TypeScript

##### 性能优化

1、源码体积优化

​	a、移除冷门feature

​	b、引入tree-shaking，减少打包体积

2、数据劫持优化

​	Object.defineProperty -> Proxy API

3、编译优化

​	通过编译阶段对静态模板的分析，编译生成Block Tree。Block tree是一个将模板基于动态节点指令切割的嵌套区块，每个区块内部的节点结构是固定的，而且每个区块只需要以一个Array来追踪自身包含的动态节点。借助Block tree，Vue.js将vnode更新性能由与模板整体大小有关提升为与动态内容的数量相关。

4、语法API优化： Composition API

​	a、优化逻辑组织

​	b、优化逻辑复用

