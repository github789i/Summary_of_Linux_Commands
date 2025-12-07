# Anaconda 常用命令与技巧 

##  1. 环境管理

### **🔹 1.1 查看与切换环境**

```bash
# 查看所有虚拟环境
conda info --envs

# 切换到某个环境
conda activate python3_7

# 退出当前环境
conda deactivate
```

### **🔹 1.2 创建环境**

```bash
conda create -n env-name python=3.8
```

### **🔹 1.3 删除环境**

```bash
conda remove -n env-name --all
```

### **🔹 1.4 配置渠道（官方源）**

```bash
conda config --add channels https://repo.continuum.io/pkgs/free/
conda config --add channels https://repo.continuum.io/pkgs/main/
conda config --set show_channel_urls yes
```

------

##  2. 设置镜像源（推荐国内源）

### **🔹 清华源（TUNA）**

```bash
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
```

### **🔹 搜索显示通道地址**

```bash
conda config --set show_channel_urls yes
```

------

##  3. 安装库（conda + pip）

### **🔹 3.1 使用 CONDA 安装**

```bash
conda install cudatoolkit=10.1
conda install cudnn=7.6
```

### **🔹 3.2 使用 pip（国内镜像）**

```bash
pip install --upgrade --ignore-installed -i https://pypi.mirrors.ustc.edu.cn/simple paddle-pipelines

# pip 指定镜像安装库
pip install -i https://pypi.mirrors.ustc.edu.cn/simple 库名

# 安装 pyinstaller
pip install -i https://pypi.mirrors.ustc.edu.cn/simple pyinstaller
```

### **🔹 3.3 打包 Python 程序（PyInstaller）**

```bash
pyinstaller --distpath C:/Users/LJG --onefile ChatAPP.py
```

### **🔹 3.4 requirements.txt 安装包**

```bash
pip install -i https://pypi.mirrors.ustc.edu.cn/simple -r requirements.txt
```

------

##  4. 查看系统与库

### **🔹 pip 查看已安装库**

```bash
pip list
pip show PyQt5
```

### **🔹 查看 GPU 信息**

```bash
nvidia-smi
```

------

##  5. 卸载库

```bash
pip uninstall torch
```

------

##  6. 环境变量 Path 示例

```bash
C:\Program Files (x86)\Common Files\Oracle\Java\javapath
```

------

##  7. VSCode Python 环境切换

### **打开命令面板**

```bash
Ctrl + Shift + P
```

### **选择解释器**

```bash
Python: Select Interpreter
```

------

##  8. 实用技巧（必须收藏 ⭐）

### **🔹 创建带指定 pip 源环境**

```bash
conda create -n env python=3.10 pip
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
```

### **🔹 克隆现有环境**

```bash
conda create -n new_env --clone old_env
```

### **🔹 导出环境（备份）**

```bash
conda env export > environment.yaml
```

### **🔹 从备份恢复**

```bash
conda env create -f environment.yaml
```

------

##  9. 开发相关快捷键（通用 + VSCode）

## 🔸 **终端常用快捷键**

| 功能               | 快捷键     |
| ------------------ | ---------- |
| 清屏               | `Ctrl + L` |
| 中断程序           | `Ctrl + C` |
| 搜索历史命令       | `Ctrl + R` |
| 显示历史命令       | `history`  |
| 重新执行上一条命令 | `!!`       |
| 返回上一个目录     | `cd -`     |

------

## 🔸 **VSCode 快捷键（高频）**

### **编辑类**

| 功能         | 快捷键              |
| ------------ | ------------------- |
| 打开命令面板 | `Ctrl + Shift + P`  |
| 复制行       | `Shift + Alt + ↑/↓` |
| 删除行       | `Ctrl + Shift + K`  |
| 格式化代码   | `Shift + Alt + F`   |

### **运行与调试**

| 功能                    | 快捷键                                         |
| ----------------------- | ---------------------------------------------- |
| 打开终端                | `Ctrl + Shift + ``                             |
| 运行代码（Python 插件） | `Ctrl + F5`                                    |
| 切换解释器              | `Ctrl + Shift + P` → 输入 `Python Interpreter` |