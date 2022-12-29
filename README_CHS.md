# RBTray

RBTray 是一个运行在后台的很小的 Windows 程序，通过以下方式使几乎任何窗口最小化进系统托盘：

- `右键单击` 窗口的最小化按钮
- `Shift + 右键单击` 窗口的标题栏（title bar）
- 使用快捷键 `Ctrl + Alt + ↓` 

请注意，以上的每一种方式不一定能在每一个窗口都有效，所以请使用任何一种有效的方式满足你的需求。

RBTray 是自由，开源的，发布在 [GNU General Public Licence](http://www.gnu.org/copyleft/gpl.html) 条款下。

## 下载

从这里下就行了：https://github.com/benbuck/rbtray/releases
- [64 位二进制文件](x64)
- [32 位二进制文件](x86)
- [源 RBTray](https://sourceforge.net/projects/rbtray/files/)

## 安装

根据您的系统，下载 `32位` 或者 `64位` 二进制文件进一个文件夹，例如 "`C:\Program Files\RBTray`"。
双击 `RBTray.exe` 开始运行。如果您想其在您重启电脑后自动运行，请在您的开始菜单启动组中创建一个 `RBTray.exe` 的快捷方式。

On Windows 10 that is located at
`"C:\Users\YOUR_USERNAME_HERE\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup"`

But a **_much_** quicker way to access it is to press "`WIN` + `R`" then type
(or copy & paste) `shell:Startup`

## 使用

To minimize a program to the system tray, you can use any of these methods:

- Right-click with the mouse on the program's minimize button.
- Hold down a Shift key while right-clicking on the program's title bar.
- Pressing Control-Alt-Down on the keyboard (all at the same time).

This should create an icon for the window in the system tray. To restore the
program's window, single-click the program's icon in the tray. Alternatively,
you can right-click on the tray icon which will bring up a popup menu, then
select **Restore Window**.

In some cases, the first two methods cause problems with other software because
of they way they integrate into Windows using a hook to intercept mouse events.
In these cases, you can use the `--no-hook` option, which means that only the
last method of using the Control-Alt-Down hotkey will work. Also in this case
the RBHook.dll isn't needed since it only exists to support the mouse event
hook.

## 退出

Right-click on any tray icon created by RBTray and click **Exit RBTray** in the
popup menu, or run RBTray.exe with the `--exit` parameter.

## 作者

Nikolay Redko: <http://rbtray.sourceforge.net/>, <https://github.com/nredko>

J.D. Purcell: <http://www.moitah.net/>, <https://github.com/jdpurcell>

Benbuck Nason: <https://github.com/benbuck>

## 贡献者

Dimitri Pappas <https://github.com/fragtion>

Ondrej Petrzilka <https://github.com/OndrejPetrzilka>

Andrzej Włoszczyński <https://github.com/Andrzej-W>

Hugo Locurcio <https://github.com/Calinou>

## 其他

For original forum, bug tracker, etc. see [RBTray SourceForge project page]
(<http://sourceforge.net/projects/rbtray/>).

Copyright &copy; 1998-2011 Nikolay Redko, J.D. Purcell

Copyright &copy; 2015 Benbuck Nason
