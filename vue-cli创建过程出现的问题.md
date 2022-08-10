![image-20220714145334967](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714145334967.png)

这个报错是 当该路径中 已经存在同名文件夹时，会出现的提示

1. 覆盖已经存在的文件夹
2. 进行文件夹之间的合并
3. 取消创建



在组件的命名中 我们需要进行多个单词进行组成

**比如 my_test.vue			My_Test.vue	这样的**

但是 my-test.vue			  My-test.vue      会报错

之后 需要仔细看下我们的组件名



npm加载nanoi

npm i nanoid



引入 nanoid 的库

import {nanoid} from 'nanoid'

![image-20220714154530295](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714154530295.png)

使用for...in...去遍历的过程

将其显示在我们的界面中 我们需要使用的是id和name



我们去试试 props 

父组件给子组件一些数据

比如 我们给子组件一个data中的youName

![image-20220714155644832](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714155644832.png)



我们找到子组件 test

使用v-bind给它绑定一个值 进行传输

​	![image-20220714155720390](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714155720390.png)



在子组件中接收并且进行使用

![image-20220714155810364](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714155810364.png)

![image-20220714155821917](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714155821917.png)

这样就可以从父组件中 给子组件传递一些数据或者列表

我们还得注意 名字相同也不行，会出现如下的错误

**27:26  error  Duplicated key 'list'  vue/no-dupe-keys**

![image-20220714160121739](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714160121739.png)

接收

![image-20220714160136679](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714160136679.png)

使用

![image-20220714160151374](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20220714160151374.png)