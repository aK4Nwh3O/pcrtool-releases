# 第三方组件声明 / Third-Party Notices

本软件（PCR 打轴工具 / pcrtool）在分发时包含以下第三方组件。
这些组件的版权归各自作者所有，并分别适用其原始许可条款。
本文件不改变、也不替代任何第三方组件的许可。

本软件自身业务代码的著作权归本项目作者所有，其分发不构成对下列组件许可条款的变更。

---

## 1. Frida

- **用途**：设备侧动态插桩运行时（本软件用于在自有/授权设备上进行自动化操作与调试）
- **版本**：Node.js 绑定 `frida` 17.18.0；随包分发的设备端 server 二进制基于 Frida 17.x 构建并重命名
- **许可**：wxWindows Library Licence, Version 3.1
- **项目主页**：https://github.com/frida/frida
- **许可全文**：https://github.com/frida/frida/blob/main/COPYING

> wxWindows Library Licence 3.1 基于 GNU Library General Public Licence v2（或更新版本），
> 并附有「例外条款」，允许以二进制形式、按分发者自己的条款进行链接与再分发。
> 该例外条款 **不** 覆盖以 GPL/LGPL 许可代码为基础新增的部分。

**许可文本全文（Frida 17.x）**：

```
wxWindows Library Licence, Version 3.1
======================================

Copyright (c) 1998-2005 Julian Smart, Robert Roebling et al

Everyone is permitted to copy and distribute verbatim copies
of this licence document, but changing it is not allowed.

WXWINDOWS LIBRARY LICENCE
TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION

This library is free software; you can redistribute it and/or modify it
under the terms of the GNU Library General Public Licence as published by
the Free Software Foundation; either version 2 of the Licence, or (at your
option) any later version.

This library is distributed in the hope that it will be useful, but WITHOUT
ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
FOR A PARTICULAR PURPOSE.  See the GNU Library General Public Licence for
more details.

You should have received a copy of the GNU Library General Public Licence
along with this software, usually in a file named COPYING.LIB.  If not,
write to the Free Software Foundation, Inc., 51 Franklin Street,
Fifth Floor, Boston, MA 02110-1301 USA.

EXCEPTION NOTICE

1. As a special exception, the copyright holders of this library give
   permission for additional uses of the text contained in this release of
   the library as licenced under the wxWindows Library Licence, applying
   either version 3.1 of the Licence, or (at your option) any later version
   of the Licence as published by the copyright holders of version 3.1 of
   the Licence document.

2. The exception is that you may use, copy, link, modify and distribute
   under your own terms, binary object code versions of works based on the
   Library.

3. If you copy code from files distributed under the terms of the GNU
   General Public Licence or the GNU Library General Public Licence into a
   copy of this library, as this licence permits, the exception does not
   apply to the code that you add in this way.  To avoid misleading anyone
   as to the status of such modified files, you must delete this exception
   notice from such code and/or adjust the licensing conditions notice
   accordingly.

4. If you write modifications of your own for this library, it is your
   choice whether to permit this exception to apply to your modifications.
   If you do not wish that, you must delete the exception notice from such
   code and/or adjust the licensing conditions notice accordingly.
```

**获取对应源码**：Frida 及其设备端 server 的完整源码可从上述项目主页获取。
如需本软件所分发的设备端二进制的**精确构建对应源码**（含重命名等构建期改动说明），
请通过本仓库 Issues 提出请求，我们将在合理时间内提供。

---

## 2. Node.js

- **用途**：程序内嵌的脚本运行时（`node.exe`）
- **许可**：MIT License，并包含若干第三方组件的许可（详见其发行版 `LICENSE` 文件）
- **项目主页**：https://github.com/nodejs/node
- **许可全文**：https://github.com/nodejs/node/blob/main/LICENSE

```
Copyright Node.js contributors. All rights reserved.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to
deal in the Software without restriction, including without limitation the
rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
sell copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
IN THE SOFTWARE.
```

---

## 3. Android SDK Platform Tools (adb)

- **用途**：与 Android 设备/模拟器通信（`adb.exe`、`AdbWinApi.dll`、`AdbWinUsbApi.dll`）
- **版权**：Copyright (C) 2012 The Android Open Source Project
- **许可**：Apache License 2.0
- **项目主页**：https://android.googlesource.com/platform/packages/modules/adb
- **许可全文**：https://www.apache.org/licenses/LICENSE-2.0

```
Copyright (C) 2012 The Android Open Source Project

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

---

## 4. Tauri

- **用途**：桌面应用框架
- **许可**：MIT License / Apache License 2.0（双许可）
- **项目主页**：https://github.com/tauri-apps/tauri

---

## 5. 其他 npm 依赖

本软件捆绑的 JavaScript 运行时依赖（如 `xlsx`、`jszip` 及其传递依赖）各自适用其原始许可，
其完整清单可通过程序安装目录内 `node_modules` 下的 `package.json` 与 `LICENSE` 文件查阅。

---

## 联系与源码请求

如你是上述组件的版权持有人，或需要获取本软件所分发二进制的对应源码，
请在本仓库 Issues 提出，我们将及时响应。

> 本文件仅为组件归属说明，不构成法律意见。
