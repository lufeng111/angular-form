# AngularForm

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.1.0.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

## angular 有两种表单处理方式
<!-- 
模板式表单：
  表单的数据模型是通过组件模板中的相关指令来定义的，因为使用这种方式定义表单的数据模型时，我们会受限于html的语法，所以，模板驱动的方式只适用于一些简单的场景

响应式表单：
  使用响应式表单时，你通过编写typeScript代码来创建一个底层的数据模型，在这个模型定义好以后，使用一些特定的指令，将模板上的html元素与底层的数据模型连接在一起

模板式表单 和 响应式表单的不同点：
  不管哪种表单，都有一个对应的数据模型来存储表单的数据，在模板表单中，数据模型是由angular基于你组件模板中的指令隐式创建的，而在响应式表单中，你通过编码明确的创建数据模型然后将模板上的html元素和底层数据模型连接在一起。

数据模型并不是一个任意的对象，它是一个有angular/forms模块中的一些特定关系的类，如FormControl, FormGroup,FormArray等组成，在模板式表单中，你是不能直接访问到这些类的，

响应式表单并不会替你生成html, 模板仍然需要你自己来写，

注意：不管使用哪种表单都需要引入angular的模块
模板式表单需要引入：FormsModule
响应式表单需要引入：ReactiveFormsModule

纯html表单:
  显示表单项
  效验用户输入
  提交表单数据
 -->

## 模板式表单
<!-- 
使用模板式表单时，只能使用指令来定义数据模型：这三个指令都来自于FormsModulemokau
  NgForm: 指令用来代表整个表单，在angular应用里会自动的添加到每个form标签上，而且NgForm指令 隐式的创建一个FormGroup类的实例，FormGroup 用来代表表单的数据模型，并且存储表单的数据， 在模板上标有NgForm指令的form标签会自动发现其标有NgModel 指令的子元素，并将他们的值添加到表单的数据模型中，
  注意：NgForm标签可以在form标签之外使用，

  NgModel

  NgModelGroup：代表的是表单的一部分，它允许你将表单的字段组织在一起，形成更清晰的层次关系，与ngForm 这个指令类似，NgModelGroup这个指令也会隐式的创建一个FormGroup类的实例，这个实例会在ngForm对象的value属性中表现为一个嵌套的对象，所以NgModelGroup的子属性都会变为嵌套对象的子属性，





 -->
