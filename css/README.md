大标题
======


二标题
------

  单独用三个`=`　`-` `*` `_`　可以显示实线或虚线

### 标题
\# 一级标题<br>
\## 二级标题<br>
\### 三级标题<br>
\#### 四级标题<br>
\##### 五级标题<br>
\###### 六级标题<br>

### 普通文档
Hello， 我要换行
换行
换行
换行失败
#### 换行请用\<br>
Hello，我要再次换行<br>
换行<br>
换行<br>
换行成功

#### 超链接URL
https://github.com/FHeaven/study-notes

#### 输出空格请用全角空格
Hello,　　　how are you!

#### 使用两个tab显示单行文档
    单行文档

#### 使用两个tab显示多行文档
    多行文档
    多行文档
    多行文档

### 超链接
[CSS Study](https://github.com/FHeaven/study-notes/new/master/css "CSS Study")  

### 使用\*和Tab可以做出多级缩进的标题
* 一级
  * 二级
    * 三级

### 插入网络图片
##### 有Mouse over
![](http://www.baidu.com/img/bdlogo.gif "百度logo")
##### 没有Mouse over
![](http://www.baidu.com/img/bdlogo.gif)

### 插入网络图片有超连接
[![baidu]](http://baidu.com)  
[baidu]:http://www.baidu.com/img/bdlogo.gif "百度Logo"  

### 插入代码（java, typescript, javascript, c）
```typescript
import { RxJsDemoComponent } from './rxjs-demo/rxjs-demo.component';
import { CommonComponentModule } from './../common-component/common-component.module';
import { InputsOutputsComponent } from './inputs-outputs/inputs-outputs.component';

import { CommonModule } from '@angular/common';
import { SampleRoutingModule } from './sample-routing.module';
import { DatePipeDemoComponent } from './pipe-demo/date-pipe-demo/date-pipe-demo.component';

import { FormsModule } from '@angular/forms';
import { NgModule } from '@angular/core';

@NgModule({
    imports: [
        FormsModule,
        SampleRoutingModule,
        CommonModule,
        CommonComponentModule
    ],
    declarations: [
        DatePipeDemoComponent,
        InputsOutputsComponent,
        RxJsDemoComponent
    ],
    exports: [],
    providers: []
})
export class SampleModule {}

```
