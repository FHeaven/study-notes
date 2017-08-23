### 普通文档
Hello， 我要换行
换行
换行
换行失败


### 超链接
[我的博客](https://github.com/FHeaven/study-notes/new/master/css "悬停显示")  

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
