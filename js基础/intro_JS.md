#JS:
###     一：
         前端用户的交互利器
         使网页更具交互性，给站点的用户提供更好、更令人兴奋的体验
         JavaScript还可以处理表单、设置cookie、即时构建HTML页面以及创建基于Web的应用程序。
###     二：
         js不允许读取客户机上的文件；但是js可以写cookie到客户机中，有限制。
         js不允许写服务器机器上的文件。
         js不能关闭不是由它自己打开的窗口。
         js不能从来自另一个服务器的已经打开的网页中读取信息。

###     三：
         它是基于原型面向对象的编程脚本语言：可以面向对象编程！！

         什么是原型？
                 当你用到Window.prototype时会发现是一个当前页面的整体对象。这就是原型
                 也即是最外面的"prototyp"。当然下面的子对象还有对象，对象下面还有prototype
                 。
                 很明显Window是主对象，window下面有一个构造方法constructor.constructor返回的就是window实例化对象，
                 默认初始化是就是默认对象
                 prototype: Window（这是Window对象下面的原型值，就是指向window本身）。
                 这也就是为什么
                 Window.prototyp.TEMPORARY和Window.TEMPORARY结果是一样的
                 null是没有原型的所以是最顶层的，
                 https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Inheritance_and_the_prototype_chain

###     四：
         弱类型的语言：

         值类型：

             number{==数符型==  int，float。。。。只要是数字}

             string{==字符串型== char，string }

             boolean{布尔型  true,false}

             undefined{没赋值定义型 }

             null{空类型  }


             注意点：
             undefined | null | 0 | '' 在作为逻辑判断时都是false


             类型转换：
             ”+“拼接意味
             " * 或者 / 或者 - "是算术的意味
             当然数字符型的数字能当成值（数）来算术运算，非数的字符自能拼接


             1+'a'='1a'
             1*'a'=NaN
             2*'3'=6
             5/0=infinity
        逻辑运算符：

             "==","==="分别是"值等"，"值和类型都等"


             注意点：
             switch判断是严格型

        数组和对象：

         var a=new Array(2);

###     五：
             作用域：
                 从里面往外寻找需要的变量。正如原型链的模型，我们想顶层寻找变量或属性，直至到null截止或找到为止！！！
                 （MDN-当试图访问一个对象的属性时，它不仅仅在该对象上搜寻，还会搜寻该对象的原型，以及该对象的原型的原型，依次层层向上搜索，
                 直到找到一个名字匹配的属性或到达原型链的末尾）
                 作用域目前主要是 function作用域  和  全局作用域！！！
