# OrangeFox 动作构建器
使用 Github Action 从 OrangeFox Recovery 编译您的第一个自定义恢复系统。

# 如何使用
1. 复制这个仓库。

2. 前往 `Actions` 标签 > `All workflows` > `OrangeFox - Build` > `Run workflow`，然后填写所有所需信息：
 * MANIFEST_BRANCH（`12.1` 和 `11.0`）
 * DEVICE_TREE（您的设备树仓库链接。）
 * DEVICE_TREE_BRANCH（您的设备树仓库分支。）
 * DEVICE_PATH（`device/vendor/codename`）
 * DEVICE_NAME（您的设备代号）
 * BUILD_TARGET（`boot`, `recovery`, `vendorboot`）

# 注意
* 此动作现在只支持 12.1 和 11.0 版本的清单，因为所有低于 11.0 版本的 OrangeFox 清单都被认为是过时的。
* 确保您的树使用了 OrangeFox 中的正确变量（更新的变量）；[fox_11.0](https://gitlab.com/OrangeFox/vendor/recovery/-/blob/fox_11.0/orangefox_build_vars.txt) 和 [fox_12.1](https://gitlab.com/OrangeFox/vendor/recovery/-/blob/fox_12.1/orangefox_build_vars.txt)，以避免构建错误。
