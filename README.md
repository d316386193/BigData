# BigData

这个仓库包含一个指向 [fiddler-everywhere-patch-automated](https://github.com/auto-yui-patch/fiddler-everywhere-patch-automated) 的子模块。

This repository contains a submodule pointing to [fiddler-everywhere-patch-automated](https://github.com/auto-yui-patch/fiddler-everywhere-patch-automated).

## 如何克隆这个仓库 | How to Clone This Repository

### 方法 1：克隆时自动初始化子模块（推荐）| Method 1: Clone with Automatic Submodule Initialization (Recommended)

使用 `--recursive` 参数克隆仓库，这将自动初始化并更新所有子模块：

Clone the repository with the `--recursive` flag to automatically initialize and update all submodules:

```bash
git clone --recursive https://github.com/d316386193/BigData.git
```

### 方法 2：分步克隆 | Method 2: Step-by-Step Clone

如果您已经克隆了仓库但没有使用 `--recursive` 参数，可以按以下步骤初始化子模块：

If you've already cloned the repository without the `--recursive` flag, follow these steps to initialize the submodules:

```bash
# 克隆主仓库 | Clone the main repository
git clone https://github.com/d316386193/BigData.git

# 进入仓库目录 | Enter the repository directory
cd BigData

# 初始化子模块配置 | Initialize submodule configuration
git submodule init

# 拉取子模块内容 | Fetch submodule content
git submodule update
```

### 方法 3：一条命令初始化子模块 | Method 3: One Command to Initialize Submodules

如果您已经克隆了主仓库，可以使用以下命令初始化并更新所有子模块：

If you've already cloned the main repository, use this command to initialize and update all submodules:

```bash
git submodule update --init --recursive
```

## 子模块信息 | Submodule Information

- **路径 | Path**: `project`
- **仓库 | Repository**: https://github.com/auto-yui-patch/fiddler-everywhere-patch-automated.git

## 更新子模块 | Update Submodules

要更新子模块到最新版本，使用以下命令：

To update the submodule to the latest version, use:

```bash
git submodule update --remote --merge
```

## 注意事项 | Notes

- 子模块是独立的 Git 仓库，有自己的提交历史
- 主仓库只记录子模块的特定提交 SHA
- 修改子模块需要在子模块目录内提交更改

- Submodules are independent Git repositories with their own commit history
- The main repository only records a specific commit SHA of the submodule
- To modify a submodule, commit changes within the submodule directory
