#### Angular 2 & Ionic 2 资料汇总

![](https://raw.githubusercontent.com/tigercosmos/webImg/master/angular-2-ionic-2-home.jpg)

**Angular 2 - 组件学习路线(仅供参考)**

- [Angular 2 Template Syntax & Common Directives](https://segmentfault.com/a/1190000008625978)
  - 了解 Angular 2 模板语法和常用内建指令
- [Angular 2 Directive](https://segmentfault.com/a/1190000008626070)
  - 了解指令与组件的区别及Metadata信息
- [Angular 2 Directive Lifecycle](https://segmentfault.com/a/1190000008716308)
  - 了解常用的 ngOnInit、ngOnChanges、ngAfterViewInit、ngAfterContentInit 声明周期钩子和触发顺序
- [Angualr 2 constructor & ngOnInit](https://segmentfault.com/a/1190000008685752)
  - 了解 constructor 与 ngOnInit 钩子的应用场景
- [Angular 2 ViewEncapsulation](https://segmentfault.com/a/1190000008677532)
  - 了解 ViewEncapsulation 三种封装模式的区别
- [Angular 2 Input](https://segmentfault.com/a/1190000008780672)
  - 了解 @Input() 装饰器的用法，掌握如何实现父->子组件通信
- [Angular 2 Output](https://segmentfault.com/a/1190000008794323)
  - 了解 @Output() 装饰器的用法，掌握如何实现子->父组件通信
- [Angular 2 ViewChild & ViewChildren](https://segmentfault.com/a/1190000008695459)
  - 了解 @ViewChild()、@ViewChildren() 装饰器用法，掌握如何获取子组件
- [Angular 2 ContentChild & ContentChildren](https://segmentfault.com/a/1190000008707828)
  - 了解 @ContentChild()、@ContentChildren() 装饰器用法及与@ViewChild()、@ViewChildren() 装饰器的区别
- [Angular 2 HostListener & HostBinding](https://segmentfault.com/a/1190000008878888)
  - 了解宿主元素的概念及 @HostListener()、@HostBinding() 装饰器的作用
- [Angular 2 ElementRef](https://segmentfault.com/a/1190000008653690)
  - 了解 ElementRef 的作用、定义及应用、Renderer API 常用方法
- [Angular 2 TemplateRef & ViewContainerRef](https://segmentfault.com/a/1190000008672478)
  - 了解 TemplateRef 及 ViewContainerRef 的应用
- [Angular 2 Components Communicate](https://segmentfault.com/a/1190000008959575)
  - 了解组件通信的常用方式
- Angular 2 Component Inheritance 
  - 了解组件继承相关知识
- [Angular 2 Change Detection - 1](https://segmentfault.com/a/1190000008747225)、[Angular 2 Change Detection - 2](https://segmentfault.com/a/1190000008754052)
  - 了解 Angular 2 变化检测、组件变化检测器及OnPush 策略、Mutable & Immutable、ChangeDetectorRef、Observables 等内容

**Angular 2 vs Angular 1**

- [Angular 2 NgModule vs Angular 1 module](https://segmentfault.com/a/1190000008938966)
  - 涉及 Angular 1.x 根模块、子模块及 Angular 2 根模块、根组件、子组件的定义使用


- [Angular 2 Service vs Angular 1 Service](https://segmentfault.com/a/1190000008936740)
  - 涉及 Angular 2 和 Angular 1 如何定义 service及使用方式
- [Angular 2 Pipe vs Angular 1 filter](https://segmentfault.com/a/1190000008937627)
  - 涉及 Angular 自定义管道(过滤器)、管道(过滤器)传参、管道对象($filter) 服务的使用
- [Angular 2 ngFor vs Angular 1 ng-repeat](https://segmentfault.com/a/1190000008938059)
  - 涉及 Angular *ngFor(ng-repeat) 指令使用、index($index)、trackBy(track by ) 的应用的区别
  
**Provider**

- [Angular 2 Provider](https://segmentfault.com/a/1190000008626130)
  - 涉及 useClass、useValue、useExisting、useFactory 及 Provider 使用方式
- [Angular 2 Multi Providers](https://segmentfault.com/a/1190000008626215)
  - 涉及 multi provider 作用及 Angular 2 内部应用
- [Angular 2 Forward Reference](https://segmentfault.com/a/1190000008626276)
  - 涉及 forwardRef 的作用及内部工作原理，同时解释 JavaScript 解释器不能自动提升 Class
- [Angular 2 OpaqueToken & InjectionToken](https://segmentfault.com/a/1190000008626348)
  - 涉及使用字符串作为 Token存在问题，详细介绍如何使用 OpaqueToken、InjectionToken 解决问题
  
**Directive**

- [Angular 2 Template Syntax & Common Directives](https://segmentfault.com/a/1190000008625978)
  - 涉及模板语法、常用指令简介及 NgStyle 指令解析、*ngFor trackBy 应用等
- [Angular 2 Directive](https://segmentfault.com/a/1190000008626070)
  - 涉及指令分类、Angular 2 内置属性指令、结构指令、`*directive` 结构指令语法糖、自定义属性指令、结构指令等
- [Angular 2 Directive Lifecycle](https://segmentfault.com/a/1190000008716308)
  - 涉及指令与组件的区别、指令生命周期钩子的作用及调用顺序、生命周期钩子详解、Angular 2 LifecycleHooks、SimpleChanges 相关接口等
- [Angular 2 Components Communicate](https://segmentfault.com/a/1190000008959575)
  - 涉及组件通信的常用方式：@Input、@Output、@ViewChild、模板变量、MessageService、Broadcaster (Angular 1.x $rootScope 中 $on、$broadcast ) 和 Pub - Sub 模式、RxJS Subject 存在的问题
- [Angular 2 Pass Async Data](https://segmentfault.com/a/1190000008986205)
  - 涉及父子组件通信时，处理异步输入属性的方案
- [Angular 2 Component Inheritance](https://segmentfault.com/a/1190000008976996)
  - 涉及面向对象中类和继承的概念及Angular 2 组件继承的应用及注意事项

**Decorator**

- [Angular 2 Decorator - 1](https://segmentfault.com/a/1190000008626417)
  - 涉及装饰器定义和分类、TypeScript 类装饰器、属性装饰器、方法装饰器、参数装饰器等
- [Angualr 2 Decorator - 2](https://segmentfault.com/a/1190000008626579)
  - 涉及 Angular 2 类装饰器、属性装饰器、方法装饰器、参数装饰器示例
- [Angular 2 Decorator - 3](https://segmentfault.com/a/1190000008626625)
  - 涉及 Angular 2 Metadata 分类：annotations、design:paramtypes、propMetadata、parameters 及映射关系
- [Angular 2 Input](https://segmentfault.com/a/1190000008780672)
  - 涉及 @Input、@Input('bindingPropertyName')、@Component() - inputs、setter & getter 、ngOnChanges 等
- [Angular 2 Output](https://segmentfault.com/a/1190000008794323)
  - 涉及 @Output、@Output('bindingPropertyName')、@Component() - outputs、Two-Way Data Binding、[()] 语法示例、ngModel 等 
- [Angular 2 Inject Decorator](https://segmentfault.com/a/1190000008634359)
  - 涉及 @Inject 装饰器的作用、实际应用及内部实现，并解释了非 Type 类型的参数只能用 @Inject(Something) 的方式注入的原因，此外还介绍了 @Injectable、Reflect API 等
- [Angular 2 ViewChild & ViewChildren](https://segmentfault.com/a/1190000008695459)
  - 涉及 @ViewChild、@ViewChildren 装饰器使用及 @ViewChild 装饰器原理详解
- [Angular 2 ContentChild & ContentChildren](https://segmentfault.com/a/1190000008707828)
  - 涉及 @ContentChild、@ContentChildren 装饰器使用及 @ContentChild 接口及装饰器，同时介绍了  Content Projection (内容投影) 的概念及 @ContentChild 与 @ViewChild 装饰器的区别等
- [Angular 2 HostListener & HostBinding](https://segmentfault.com/a/1190000008878888)
  - 涉及 Host Element、HostListener 装饰器定义及应用、Host  Event Listener、HostBinding 装饰器定义及应用、Host Property Bindings 等

**Pipe**

- [Angular 2 Pipe](https://segmentfault.com/a/1190000008646187)
  - Angular 2 内建管道分类及使用示例、管道参数、管道链、自定义管道、管道分类、管道探秘等
- [Angular 2 AsyncPipe](https://segmentfault.com/a/1190000008759314) 
  - 涉及 AsyncPipe with Promise、AsyncPipe with Observables、使用 AsyncPipe 重复发送请求的解决方案及 AsyncPipe 内部执行流程 (源码解析)

**Dependency Injection**

- [Angular 2 DI - IoC & DI - 1](https://segmentfault.com/a/1190000008626680)
  - 涉及 IoC 和 DI、DI 在 angular 1.x 中的应用、内部工作原理及存在的问题等
- Angualr 2 DI - 2 (未完成)

**Change Detection**

- [Angular 2 Change Detection - 1](https://segmentfault.com/a/1190000008747225)
  - 涉及变化和变化触发源、Zones、NgZone 及如何访问 Zone 打补丁前的方法，如 setTimeout、clearTimeout 等
- [Angular 2 Change Detection - 2](https://segmentfault.com/a/1190000008754052)
  - 涉及组件和变化检测器、OnChanges、变化检测性能优化、OnPush 策略、Mutable & Immutable、ChangeDetectorRef、Observables 等
  
**Http**

- [Angular 2 Http Module - HTTP](https://segmentfault.com/a/1190000008900299)
  - 涉及 B/S、URI、MIME、HTTP请求和响应报文、HTTP 请求方法和状态码，并收录了 HTTP 经典教程和相关工具，如 Cookie 与 Session、HTTP 缓存、CORS、HTTP/2、HTTPS及常用的HTTP抓包工具、Chrome相关插件、各平台HTTP包、压力测试工具等
- [Angular 2 Http Module - XMLHttpRequest](https://segmentfault.com/a/1190000008950789)
  - 涉及 AJAX、XMLHTTP、XMLHttpRequest详解、XMLHttpRequest Level 1、Level 2 详解、XHR 上传、下载数据、XHR 流式传输、XHR 定时轮询和长轮询区别与优缺点、XMLHttpRequest 常用代码片段、常见问题等
- [Angular 4.x HttpModule 脑图(思维导图)](https://juejin.im/entry/58ea34eda22b9d0058a59836/detail)
- [Angular 4.x HttpModule Reveal](https://segmentfault.com/a/1190000009028150)
  - 涉及 HTTP 协议、HTTP 请求报文、HTTP 响应报文、HttpModule Request、Response、RequestOptions、ResponseOptions、XHRBackend 对象等
- Angular 2 Http Interceptor (未完成)

**Form**

- [Angular 4.x Template Driven Forms](https://segmentfault.com/a/1190000009037539) 
  - 涉及 ngModel、[ngModel]、[(ngModel)]、ngModelGroup、Template-Driven error validation
- [Angular 4.x Reactive Forms](https://segmentfault.com/a/1190000009041192)
  - 涉及 FormControl、FormGroup、Reactive Submit、Reactive Forms error validation、FormBuilder
- [Angular 4.x 基于AbstractControl自定义表单验证](https://segmentfault.com/a/1190000009045615)
  - 涉及 FormGroup、FormBuilder与FormGroup源码、AbstractControl、自定义验证规则等
- Angular 4.x Custom Form Controls (未完成)
- Angular 4.x Custom Validators (未完成)

**Compiler**

- [Angular 2 JIT vs AOT](https://segmentfault.com/a/1190000008739157) 
  - 涉及 Just-In-Time & Ahead-Of-Time、JIT vs AOT 、AOT 详解、AOT 实战等 
- Angular 2 Compiler (未完成)

**Reference Object**

- [Angular 2 ElementRef](https://segmentfault.com/a/1190000008653690)
  - 涉及 ElementRef 的作用、定义及应用、Renderer API 常用方法
- [Angular 2 TemplateRef & ViewContainerRef](https://segmentfault.com/a/1190000008672478)
  - 涉及 HTML 5 template、TemplateRef 及 ViewContainerRef 的应用，此外介绍了 Angular 2 视图类型、ViewRef 与 EmbeddedViewRef 之间的关系等
  
**RxJS**

- [Functional Programming](https://segmentfault.com/a/1190000008794344)

  - 涉及函数式编程概念、基础条件、重要特性、优势、常用方法等

- [Observable](https://segmentfault.com/a/1190000008809168)

  - 涉及观察者、迭代器模式、Observable提案、自定义Observable、Create Operators、Observer、

    Pull vs Push、Observable vs Promise 等

- [Operators](https://segmentfault.com/a/1190000008834251) 
  - 涉及 Marble diagrams、Create Operators、Transformation Operators、Filtering Operators、Combination Operators、Utility Operators 等
- [Subject](https://segmentfault.com/a/1190000008886598)
  - 涉及观察者模式定义、结构及实战、Observable subscribe、自定义 Subject、RxJS Subject、Angular 2 RxJS Subject 应用、BehaviorSubject、ReplaySubject、AsyncSubject 等

**Others**

- [Angular 2 ViewEncapsulation](https://segmentfault.com/a/1190000008677532)
  - 涉及 Web Components、Shadow DOM 及 ViewEncapsulation 三种封装模式的区别
- [Angualr 2 constructor & ngOnInit](https://segmentfault.com/a/1190000008685752)
  - 涉及 constructor、ngOnInit、constructor & ngOnInit 应用场景等
- [Angular 2 DomSanitizer](https://segmentfault.com/a/1190000008809095)
  - 涉及 Cross-site scripting、Angular 2 XSS 防护、DomSanitizer、自定义 keepHtml 指令等


**Angular 2 - 优秀博客(英文)**

* [thoughtram](https://blog.thoughtram.io/all/)
* [toddmotto](https://toddmotto.com/)
* [nrwl](https://blog.nrwl.io/)
* [angular-university](http://blog.angular-university.io/)
* [scotch](https://scotch.io/tag/angular-js)
* [medium](https://medium.com/tag/angular2)



**Angular 2 - 视频资源**

* [rangle.io](https://rangle.io/resources/tags/angular-2/)
* [youtube - ng-conf](https://www.youtube.com/channel/UCm9iiIfgmVODUJxINecHQkA)
* [youtube - angular-university](https://www.youtube.com/channel/UC3cEGKhg3OERn-ihVsJcb7A)
* [youtube - ng-europe](https://www.youtube.com/channel/UCEGUP3TJJfMsEM_1y8iviSQ)
* [youtube - ng-be](https://www.youtube.com/channel/UCnMfZM2S3QgbFvOyet5PMmQ)



**Angular 2 - 问答**

* [angular2-ama-cn](https://github.com/kittencup/angular2-ama-cn)
* [stack overflow - angular 2 topics](http://stackoverflow.com/documentation/angular2/topics)



**Angular 2 - 社交**

* [Reddit](https://www.reddit.com/r/Angular2/)
* [Hacker News](https://news.ycombinator.com/news)



**Angular 2 - 工具**

* [Augury(调试工具)](https://augury.angular.io/)
* [Codelyzer(代码分析)](https://github.com/mgechev/codelyzer)
* [Lite-Server(轻量Node服务器)](https://github.com/johnpapa/lite-server)



**Angular 2 - 组件**

* [Angular Material 2](https://github.com/angular/material2)
* [Kendo-UI](http://www.telerik.com/kendo-angular-ui/components/)
* [ng2-bootstrap](http://valor-software.com/ng2-bootstrap/#/)
* [ngSemantic](https://ng-semantic.herokuapp.com/#/)
* [ng-lightning](http://ng-lightning.github.io/ng-lightning/#/components)
* [Onsen UI](https://onsen.io/v2/docs/guide/angular2/)



**Angular 2 - 跨平台开发**

* [angular-electron(桌面版)](https://github.com/angular/angular-electron)
* [ionic(mobile app)](http://ionicframework.com/)
* [nativescript-angular](https://github.com/NativeScript/nativescript-angular)
* [angular 2 and react native](http://angular.github.io/react-native-renderer/)
* [universal-windows-app](https://github.com/preboot/angular2-universal-windows-app)



**Ionic 2 - 中文文章**

* [Ionic 2 i18n 方案设计](https://github.com/semlinker/angular2-ionic2/issues/1)
* [Ionic 2 多主题、多租户构建方案探索](https://github.com/semlinker/angular2-ionic2/issues/1)
* [Ionic 2 中如何引入第三方脚本](https://github.com/semlinker/angular2-ionic2/issues/6)



**Ionic 2 - 优秀博客(英文)**

* [joshmorony - ionic-tutorials](https://www.joshmorony.com/category/ionic-tutorials/)









