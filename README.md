# pcrtool — 安装包分发仓库

本仓库仅用于分发 **PCR 打轴工具（pcrtool）** 的 Windows 安装包，**不包含源代码**。

## 下载

前往 [Releases](../../releases) 页面下载最新版本的安装包：

| 文件 | 说明 |
| --- | --- |
| `pcrtool_<version>_x64-setup.exe` | Windows x64 安装程序（NSIS） |
| `SHA256SUMS.txt` | 安装包校验值 |

## 校验安装包完整性

下载后请校验文件哈希，确认安装包未被篡改。

**PowerShell**

```powershell
Get-FileHash .\pcrtool_0.2.4_x64-setup.exe -Algorithm SHA256
```

**CMD**

```cmd
certutil -hashfile pcrtool_0.2.4_x64-setup.exe SHA256
```

输出应与 `SHA256SUMS.txt` 中对应行一致。

## 安装说明

1. 双击 `pcrtool_<version>_x64-setup.exe`
2. 若 Windows SmartScreen 提示「未知发布者」，选择「更多信息」→「仍要运行」
   （安装包未购买代码签名证书，属于正常现象，请以上面的 SHA256 校验为准）
3. 按向导完成安装，程序会安装到当前用户目录，无需管理员权限

### 环境要求

- Windows 10 / 11 x64
- 已安装并配置好 Android 模拟器（用于连接设备侧）
- 首次运行需要联网拉取运行所需的数据

## 使用范围声明

本工具仅供**学习交流**与**自有设备上的自动化操作**使用。
请勿用于任何未经授权的设备、账号或服务。使用本工具产生的一切后果由使用者自行承担。

## 第三方组件

本程序内嵌了若干开源组件（Frida、Node.js、Android Platform Tools 等），
相关许可与声明见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)。

## 问题反馈

请在本仓库的 [Issues](../../issues) 页面反馈问题，并附上：

- 程序版本号（安装包文件名中的版本）
- Windows 版本
- 复现步骤与报错信息
