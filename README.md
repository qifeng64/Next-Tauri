# 创建项目

-   `pnpm dlx create-next-app@latest`

-   ```javascript
    // next.config.mjs
    const nextConfig = {
        output: "export",
    };
    ```
-   `pnpm add -D @tauri-apps/cli`

    -   创建 rust 项目，一直回车（默认）

-   `pnpm tauri dev`

    -   启动 tauri，首次需等待下载依赖包，时间较长
    -   成功会打开一个 windows 应用窗口

-   `pnpm tauri build`
    -   在 `\src-tauri\target\release\bundle\` 目录生成 app 安装程序

# 常见配置

## 应用图标

-   `\src-tauri\icons\`
    -   存放应用图标
-   tarui.config.json 中 tauri.bundle.icon 配置图标读取路径

# snippet

-   `rfc` 函数式组件基础模板
