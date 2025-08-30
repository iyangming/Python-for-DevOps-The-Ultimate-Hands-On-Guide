# Python for DevOps: 掌握实战自动化

本仓库包含我的《Python for DevOps: 掌握实战自动化》课程的所有代码和材料。如果您还没有注册，请查看下面的链接获取折扣！

### ➡️ 课程链接（附带大幅折扣 🙂）：[https://www.lauromueller.com/courses/python-devops](https://www.lauromueller.com/courses/python-devops)

**注意：** 您可以在以下仓库中找到关于Python CI/CD部分的代码：[https://github.com/lm-academy/python-devops-cicd-project](https://github.com/lm-academy/python-devops-cicd-project)

**查看我的其他课程：**

- 👉 [Helm权威课程：从入门到精通](https://www.lauromueller.com/courses/definitive-helm-course)
- 👉 [精通Terraform：从入门到专家](https://www.lauromueller.com/courses/mastering-terraform)
- 👉 [精通GitHub Actions：从入门到专家](https://www.lauromueller.com/courses/mastering-github-actions)
- 👉 [Docker和Kubernetes完全课程：从零到英雄](https://www.lauromueller.com/courses/docker-kubernetes)
- 👉 [编写更好的代码：20种代码异味及如何消除它们](https://www.lauromueller.com/courses/writing-clean-code)

## 欢迎！

我很高兴您能来到这里！本仓库包含我的Python for DevOps课程的所有代码、示例和补充材料。我的目标是为您提供实用的、真实世界的示例，帮助您掌握Python用于自动化和运维任务。

## 🚀 开始使用

要在本地运行代码示例，您需要正确设置环境。强烈建议使用虚拟环境来保持项目依赖的隔离。

**重要提示**：确保安装了**Python 3.12.9**，以便顺利跟进课程而不会遇到任何问题 😊 在本课程发布之前，Python 3.13.x存在一个bug，阻止了一些原生日志功能正常工作。希望这个问题很快会在后续的Python版本中修复，但为了确保流畅的体验，推荐使用**Python 3.12.9**。

1.  **克隆仓库**

    ```bash
    git clone https://github.com/lm-academy/python-devops.git
    cd python-devops
    ```

2.  **创建并激活虚拟环境**
    创建一个新的虚拟环境（常规名称是`.venv`）：

    ```bash
    python3 -m venv .venv
    ```

    为当前shell会话激活它：

    ```bash
    # 在macOS和Linux上
    source .venv/bin/activate

    # 在Windows上
    .venv\Scripts\activate
    ```

    您的shell提示符现在应该以`(.venv)`为前缀，表示环境已激活。

3.  **安装依赖**
    本课程所需的包列在`requirements.txt`中。使用pip安装它们：

    ```bash
    pip install -r requirements.txt
    ```

4.  **启动JupyterLab**
    许多初始讲座使用Jupyter Notebooks（`.ipynb`文件）进行交互式演示。您可以通过运行以下命令启动JupyterLab界面：
    ```bash
    jupyter lab
    ```
    这将在您的网络浏览器中打开一个新标签页，允许您浏览项目文件夹并打开任何`.ipynb`笔记本文件。

## 🧑‍💻 跟随课程学习

本仓库有两个主要分支来支持您的学习：

- **`main`分支**：此分支包含每个讲座的最终完成代码。如果您遇到困难或想查看完成的解决方案，可以将其用作参考。
- **`start`分支**：此分支专为您跟随实践讲座而设计。它包含每个课程的初始状态，包括笔记本和markdown文件，但代码块通常留给您来完成。

要切换到`start`分支并跟随我编码，请运行：

```bash
 git checkout start
```

## 📚 课程结构

该仓库按模块组织，每个模块对应课程中的一个部分。以下是您将学习的内容概述：

- **virtual-envs**：了解为什么虚拟环境至关重要，以及如何使用Python内置的`venv`模块创建和管理隔离的项目环境。

- **python-fundamentals**：掌握Python的核心构建块。本模块涵盖变量、注释、数据类型（`str`、`int`、`list`、`dict`、`set`、`tuple`）、条件语句、循环、函数（包括`*args`和`**kwargs`）、类等主题。

- **generators-decorators**：探索促进干净高效代码的高级Python特性。本节涵盖一等函数、使用`yield`的内存高效生成器，以及用于添加计时和重试等功能的强大装饰器。

- **error-handling**：通过掌握错误处理来构建弹性脚本。本模块涵盖`try...except`块、引发内置和自定义异常，以及使用上下文管理器进行安全资源管理。

- **logging**：超越`print()`语句，学习使用Python的`logging`模块。您将探索日志级别、处理程序、格式化程序、基于文件的日志记录与轮换，以及使用JSON的现代结构化日志记录。

- **files-regex-data-formats**：深入文件I/O和数据处理。您将学习使用`pathlib`处理文件系统路径，使用正则表达式（`re`）处理文本，以及处理常见的数据序列化格式，如**CSV**、**JSON**和**YAML**。

- **interacting-with-os**：编写与操作系统交互的脚本。本模块涵盖管理环境变量、使用`subprocess`执行外部命令、使用`os`和`shutil`处理文件系统操作，以及创建临时文件。

- **http-requests**：学习使用强大的`requests`库与Web服务和REST API交互。主题包括发出GET/POST请求、传递参数、处理身份验证，以及实现具有重试和超时的健壮错误处理。

- **typing**：通过Python的类型提示系统提高代码清晰度并及早捕获错误。本模块介绍来自`typing`模块的基本和高级类型、带有`TypeVar`的泛型，以及如何使用`mypy`等静态分析工具验证您的代码。

- **automated-testing**：学习如何使用pytest编写自动化测试，包括断言、参数化、标记、fixture和模拟。

- **multi-file-projects**：了解如何组织更大的Python项目，包括模块、包、子包和测试。