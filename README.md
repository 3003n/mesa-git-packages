# mesa-git-packages

自动构建最新的 mesa-git 和 lib32-mesa-git 包。每天从 mesa 上游仓库获取最新代码进行构建。

## 包含的包

- mesa-git
- lib32-mesa-git

## 自动构建

- 每天自动从 mesa 上游仓库获取最新代码进行构建
- Release tag 使用 mesa 源码的 commit hash
- Release 名称格式：`Mesa Git Build YYYYMMDD-hash`

## 安装方法

### 从最新 Release 安装

1. 访问 [Releases](../../releases) 页面
2. 下载最新的 Release 中的包文件
3. 使用 pacman 安装：

```bash
# 安装 mesa-git
sudo pacman -U mesa-git-*.pkg.tar.zst

# 安装 lib32-mesa-git（可选）
sudo pacman -U lib32-mesa-git-*.pkg.tar.zst
```

## 注意事项

- 这些包会替换官方的 mesa 和 lib32-mesa 包
- 由于使用最新的开发版本代码，可能会存在不稳定性
- 如果遇到问题，可以根据 Release tag（mesa commit hash）在 mesa 仓库中查找对应版本

## 相关链接

- [Mesa 项目](https://gitlab.freedesktop.org/mesa/mesa)
- [mesa-git AUR](https://aur.archlinux.org/packages/mesa-git)
- [lib32-mesa-git AUR](https://aur.archlinux.org/packages/lib32-mesa-git)