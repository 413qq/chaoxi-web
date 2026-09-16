# 朝夕纯网页版

适用于 GitHub Pages 的静态网页，无需聊天后台。包含温以宁、陆景珩、自定义角色、聊天、浏览器记忆和备份。

在“我的”输入自己的 DeepSeek API Key。密钥仅在当前页面内存保留，刷新需重填。聊天和记忆直接发送到 DeepSeek；模型调用消耗使用者的 API 额度。

记录只保存在当前浏览器，不提供账号登录和跨设备同步。请定期导出备份。主动搭话仅在网页前台打开时生效，锁屏和关闭网页后不会推送。

## 发布
将整个源码仓库推送至 main，在 Settings → Pages 中选择 GitHub Actions。随仓库提供的工作流发布 dist/public。

也可将 dist/public 的全部文件放入仓库根目录，选择 Deploy from a branch → main → /(root)。不要只上传 ZIP。必须通过 HTTPS 网站访问，不能只双击 HTML。

iOS 在 Safari 打开网址，通过分享菜单添加到主屏幕；安卓通过浏览器菜单添加到主屏幕。

## 构建
Node 24，执行 npm install 和 npm run build。修改源码后重新构建并提交 dist/public。

本机已验证记忆刷新保留、DeepSeek 无效密钥错误恢复。未验证实体 iPhone 或当前版本真实模型回复。网络可达性取决于访问者所在网络。

保留 OWNSEEK-LICENSE、OWNSEEK-NOTICE、THIRD-PARTY-LICENSES。
