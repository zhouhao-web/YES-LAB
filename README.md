# YES-LAB、 安装步骤简述
1. 安装虚拟机：在Windows宿主机安装 VMware Workstation 17 Pro。
2. 安装系统：下载 Ubuntu 20.04.6 ISO镜像，在虚拟机中完成安装，并设置好系统语言和用户名（zhouhao）。
3. 配置ROS源：设置软件源，安装ROS Noetic完整版。
4. 环境配置：初始化 `rosdep`，并在 `~/.bashrc` 中配置环境变量 `source /opt/ros/noetic/setup.bash`。
 三、 遇到的问题及解决办法（重点）
**问题1：在Windows PowerShell中执行 `lsb_release -a` 报错**
- **描述**：习惯性在Windows终端执行Linux命令，提示“无法将...识别为 cmdlet”。
- **解决**：明确区分Windows和Ubuntu环境。查看系统版本必须进入VMware里的Ubuntu系统终端（Ctrl+Alt+T）执行。

**问题2：终端粘贴命令时出现 `<pre>` 和 `</pre>` 标签报错**
- **描述**：从笔记或网页复制命令时，带入了HTML标签。
- **解决**：在终端粘贴前检查命令，手动删掉多余的标签字符。

**问题3：执行 `lsb_release -a` 提示 `No LSB modules are available
