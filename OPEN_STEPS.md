## 0. 说明
本文档为项目开源前所需要做的准备事宜进行步骤讲解。

## 1. 项目名字和文件结构
一个规范化的项目文件结构能够方便用户从总体上观察项目，一眼了解项目组成。

项目名字使用英文小写，使用有意义的英文单词，多个单词使用中划线'-'隔开，例如，
- hystrix
- wirelss-gate
- simple-demo
- open-source-sample

一个项目中必须包含如下文件，
- README.md
- .gitignore
- LICENSE
各个文件的编写格式请参考样例。

下面给出几个常用开发项目的文件结构，

#### Maven单模块项目文件结构

```
- pom.xml
- README.md
- LICENSE
- .gitignore
+ target
+ src
  - main/java/Hello.java
```
注：.gitignore只需在项目根目录中放置。target文件夹放置编译好的文件，无需提交到代码仓库。

#### Maven多模块项目文件结构
和单模块相比，每个子模块可以拥有自己的README文件。

```
- pom.xml
- README.md
- LICENSE
- .gitignore
+ module1
  - pom.xml
  - README.md
  + target
  + src/main/java
  + src/test/java
+ module2
  - pom.xml
  - README.md
  + target
  + src/main/java
  + src/test/java
```
注：.gitignore只需在项目根目录中放置。target文件夹放置编译好的文件，无需提交到代码仓库。

#### 前端vue项目文件结构

```
- README.md
- LICENSE
- .gitignore
- package.json
- webpack.config.js
- .babelrc
- ./postcssrc.js
- dist
- node_modules
+ src
  - index.html
  - main.js
  + components
  + pages
  + store
  + router
```
注：.gitignore只需在项目根目录中放置。dist文件夹放置编译好的文件，无需提交到代码仓库。node_modules文件夹放置第三方依赖包，无需提交到代码仓库。

## 2. 附加版权许可证（LICENSE）文件到项目根目录

项目采用Apache License 2.0， 版权许可证文件格式如下，

```
Copyright 2018 ppdai.com

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## 3. 附加README文件到各个项目目录，包括子项目
README文件的具体格式请参见本演示项目。

## 4. 附加.gitignore到项目根目录
README文件的具体格式请参见本演示项目。

## 5. 附加版权许可声明到各个源代码文件
更新所有源代码文件，附加版权许可声明，包括，
- 源代码文件.java/.js/.vue
- Java资源配置文件.xml/.yml/.properties
- Maven的构建声明文件pom.xml

下面几个特例文件可以不添加版权许可声明，
- .gitignore
- .html

source files
```
/*
 * Copyright 2018 ppdai.com
 *
 * Licensed under the Apache License, Version 2.0 (the "License");
 * you may not use this file except in compliance with the License.
 * You may obtain a copy of the License at
 *
 * http://www.apache.org/licenses/LICENSE-2.0
 *
 * Unless required by applicable law or agreed to in writing, software
 * distributed under the License is distributed on an "AS IS" BASIS,
 * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 * limitations under the License.
 */
 ```

xml files
 ```
 <!--
  Copyright 2018 ppdai.com

  Licensed under the Apache License, Version 2.0 (the "License");
  you may not use this file except in compliance with the License.
  You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

  Unless required by applicable law or agreed to in writing, software
  distributed under the License is distributed on an "AS IS" BASIS,
  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
  limitations under the License.
-->
```

properties文件
```
#
# Copyright 2018 ppdai.com
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# limitations under the License.
#
```

## 6. 源代码注释
在尽可能的情况下，为主要代码类和关键代码流程上添加注释，方便用户阅读和理解。

后端源代码需要考虑添加注释的地方，
- 每个类文件添加注释，说明类的主要功能
- 主要类方法上添加注释，说明该方法实现的主要功能
- 关键代码流程上添加注释，说明每个流程的关键点
- 配置文件

如下是一个类文件注释样例，
```
/**
 * 这是一个简单的类注释示范样例。
 * <p>
 * <p>主程序文件 <code>Hello</code> 在控制台上输出"Hello,world"。
 *
 * @author huangyinhuang
 * @version 2/10/2018
 */
```

前端源代码需要考虑添加注释的地方，
- 每个前端组件添加注释，说明组件的主要功能
- 关键代码流程上添加注释，说明每个流程的关键点
- 配置声明
