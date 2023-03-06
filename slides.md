---
theme: ./theme
highlighter: shiki
lineNumbers: false
info: vscode_cmake_cxx_tdd
drawings:
  persist: false
download: true
class: text-center
title: VSCode | CMake | C++  | TDD
layout: quote
position: center
---

<div class="text-5xl mb-12 font-bold">
  "VSCode | CMake | C++  | TDD"
</div>

<div class="pt-2 mb-16 opacity-70">
  医用开发部 - 苏佳彬
</div>

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---
layout: image-x
image: 'images/ocean.jpg'
imageOrder: 2
---

# 目录

- 📝 **CMake**
- 🧑‍💻 **配置开发环境**
- 🧪 **Demo 演示**
- 🎨 **TDD（GoogleTest）**

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---

# CMake

**跨平台**的编译工具

CMake

- 是一个主要用于 C++ 的构建工具。

- 是平台无关的中间编译工具。同一个 CMake 编译规则在不同操作系统会构建出不同的可执行构建文件。在 Linux 产生 MakeFile，在 Windows 平台产生 Visual Studio 工程 sln 等。CMake 旨在解决各平台的不同 Make 工具的产生的差异（比如 GNU Make， QT 的 qmake，微软的 nmake， BSD 的 pmake）。

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

<!--
CMake 可以用简单的语句来描述所有平台的编译过程。
-->

---
layout: image
image: '/images/cmake.png'
imageOrder: 1
---

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---
layout: image-x
image: '/images/cmake_download.png'
imageOrder: 2
---

# 配置开发环境

下载 CMake

首先，自己的电脑中需要在[官网](https://cmake.org/download/)上下载对应的 CMake 安装包。

Windows 选择 .msi 的，Linux 选择 .sh 的，都是可以直接执行后无脑安装的。

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---
layout: image-x-thin
image: '/images/vscode_plugin.png'
imageOrder: 2
---

# 配置开发环境

下载 VSCode 以及其插件

VSCode [官网](https://code.visualstudio.com/)下载即可，然后搜索以下插件进行下载。

- C/C++ 能让 .h/.hpp/.c/.cpp 文件能有语法高亮，以及可做函数查找和跳转等操作。
- Clang-Format 能配置 C/C++ 代码格式化的风格。
- CMake 能语法高亮 CMakeLists.txt 配置文件。
- CMake Tools 即 VSCode 中集成之前下载的 CMake, 可以说 CMake 的一个 UI 版本。
- cmake-format 代码格式化 CMakeLists.txt

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---

# Demo 演示

生成执行文件或生成链接库

步骤

- 编写 CMakeLists.txt 配置文件
- VSCode 下使用 CMake Tools 插件选择编译器和（debug/release）
- 直接点击 CMake Tools 提供的 build 按钮生成对应平台和对应编译器的构建文件（makefile/sln）
- 直接点击 CMake Tools 提供的 run 运行按钮或 debug 调试按钮来跑代码。

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---
layout: two-cols
---

# TDD（GoogleTest）

Test Driven Development，即测试驱动开发。

<br />

TDD 的好处

- 代码质量更高
- 代码更健壮
- 代码更容易重构
- 代码更容易维护
- 代码更容易理解
- 代码更容易扩展

::right::

<br />
<br />
<br />
<br />
<br />
<br />

TDD 的流程

- 先写测试
- 再写代码
- 重构代码

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---

# TDD（GoogleTest）

GoogleTest 是 Google 开源的一个 C++ 单元测试框架。

GoogleTest 的特点

- 轻量级
- 无侵入性
- 易于使用
- 能够生成测试报告

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---

# TDD（GoogleTest）

GoogleTest 是 Google 开源的一个 C++ 单元测试框架。

<br />

CMake 配置 GoogleTest，可查看[官网指导](https://google.github.io/googletest/quickstart-cmake.html)

具体项目说明 -- `cxx_crud_file`

<BarBottom title="VSCode | CMake | C++  | TDD">
  <Item text="医用开发部">
    <carbon:id-management />
  </Item>
  <Item text="苏佳彬">
    <carbon:user-avatar-filled-alt />
  </Item>
</BarBottom>

---
layout: end
---

END

