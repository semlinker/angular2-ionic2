### Ionic 2 项目开发说明文档

#### 一、开发规范

文件夹命名方式: `platform-browser、language-service`

文件命名方式统一使用小写英文单词，多个单词使用下滑线 (`_`) 进行分隔, 如 `common_module.ts`

1.1 命名规范  

- 控制器命名方式，文件名命名 `nav_controller.ts`,  class命名  `NavController`
- 服务命名方式，文件命名 `api_service.ts` , class命名  `ApiService`  
- 组件命名方式，文件命名 `app_component.ts` , class命名 `AppComponent`。组件的输入属性和输出属性使用驼峰方式命名：`@Iutput() tabTitle`
- 管道命名方式，文件命名`async_pipe.ts` , class 命名`AsyncPipe`
- 指令命名方式，文件命名 `ng_class.ts`, class 命名 `NgClass`。指令(组件)的 `selector` 使用 `exe-` 前缀方式命名。
- HTML文件命名方式，以小写英文单词命名，多个单词之间用"-"分隔,如`exam-card.html`
- TypeScript文件命名方式，以小写英文单词命名，多个单词之间用"_"分隔，如`user_service.ts`
- SCSS文件命名方式，以下划线开头+小写英文单词，各个单词之间使用"-"分隔，如`_nav-bar.scss`

1.2 目录规范  

项目开发的根目录为 `src `目录:  

- app  ——  存放项目入口文件，如 `app_module.ts`


- assets —— 存放项目资源文件
  - config —— 存放系统配置文件，如`API`服务器地址
  - i18n ——  存放语言包，模块(组件)相关的语言包存放于各自模块(组件)文件夹内
  - icon  ——  存放 `icon` 文件
  - images  ——  存放项目图片资源文件
  - lib  ——   存放项目依赖的第三方资源库
- core  ——   存放核心模块如`ApiService`、`AuthService` 等
- features - 存放功能模块
- shared - 存放功能模块中共享的组件、服务或管道
- pages —— 存放各个模块的 `html` 模板文件及 `ts`业务逻辑文件，根据模块建立对应的目录，如登录模块位于`pages/login` 文件下
- theme  ——  存放各个租户主题样式

1.3 Class文件规范

import文件的顺序，`@angular/*`、`ionic-angular` 、第三方依赖库、项目中依赖文件；属性名和方法名称统一使用驼峰命名，属性名必须设定对应的参数类型，同时方法也要设置输入参数类型和返回对象的类型。每个方法统一使用`Document This` 进行方法功能注释。具体示例如下：

```typescript
import { Injectable } from '@angular/core';
import { Observable } from 'rxjs/Observable';

import { ApiService } from './api_service';
import { AppConfig } from '../config/app_config';
import { aesEncrypt } from '../util/lang';
import { LoginRequestArgs } from './interfaces';
import { Platform } from './enums';

@Injectable()
export class AuthService {

    ssoUrl: string; // 登录URL地址

    verifycodeUrl: string; // 验证码URL地址

    constructor(public appConfig: AppConfig, public apiService: ApiService) {
        this.ssoUrl = appConfig.getConfig('sso');
        this.verifycodeUrl = appConfig.getConfig('verifycode');
    }

    /**
     * 验证Token是否有效,支持版本参数
     *
     * @param {string} ticket
     * @param {string} version
     * @returns {Observable<any>}
     *
     * eg:
     * validateToken("123456") => /api/Ticket?id=123456&info=1
     * validateToken("123456", "V2") => /api/Ticket/V2?id=123&info=1
     *
     * @memberOf AuthService
     */
    validateToken(ticket: string, version: string): Observable<any> {
        let baseUrl = `${this.ssoUrl}/api/Ticket{version}?id=${ticket}&info=1`;
        let validateUrl = version ?
            baseUrl.replace("{version}", `/${version}`) :
            baseUrl.replace("{version}", '');
        return this.apiService.get(validateUrl);
    }
}
```

#### 二、搭建开发环境

2.1 环境安装  

**Windows平台**

```
npm install -g cordova ionic  
安装ant
系统环境变量中配置android sdk路径
```

**iOS平台**  

```
sudo npm install -g cordova ionic   
sudo npm install -g ios-sim  
ionic platform add ios	# 添加ios平台
ionic build ios	# 构建ios项目  
ionic emulate ios	# 模拟器运行  
ionic run ios	# 连接真机后直接运行
```

模拟器运行

- 支持模拟器运行
  - npm install -g ios-sim


- 列出 iOS 设备类型
  - ios-sim showdevicetypes
- 模拟器运行
  - ionic emulate ios —target="iPad-Air"
- 开启 `livereload` 和 `console`
  - ionic emulate ios -l -c
- 开启日志(Logging)
  - consolelogs:	ionic emulate ios —c
  - serverlogs: ionic emulate ios —s
- 获取命令行信息
  - ionic info

2.2 命令行

2.2.1 初始化项目

- ionic start myApp [template name] —v2
  - template name: blank、sidemenu、tabs
- ionic start myApp -a "My Awesome Ionic App"
  - -a: appname
- ionic start myApp -i com.mycompany.appname
  - -i: app id

2.2.2 定义构建的平台

- ionic platform add [platform name]
  - platform name: ios、android、windows
- ionic platform remove [platform name]

2.2.3 插件管理

- ionic plugin add [plugin id] # 添加插件
- ionic plugin rm [plugin id] # 移除插件
- ionic plugin ls # 列出已安装的插件

2.2.4 ionic 生成器

- ionic g [page|component|directive|pipe|provider|tabs]

2.2.5 预览应用程序

- ionic serve
  - ionic serve —lab 在浏览器中同时预览 iOS、Android、Window 平台

2.3 Visual Studio Code 常用插件

- Auto Import
- Debugger for Chrome
- Document This
- Material Theme
- Rainbow Brackets
- Beautify
- Auto Rename Tag
- Git History
- HTML Snippets
- Path Intellisense
- Angular 2 TypeScript Snippets - Johnpapa
- Angular 2 TypeScript Emmet
- Ionic 2 Commands with Snippets
- ESLint
- Code Runner
- HTML CSS Class Completion
- JavaScript(ES 6) code snippets
- REST Client