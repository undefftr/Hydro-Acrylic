# Hydro-Acrylic
适用于Hydro的卡片模糊与自定义背景插件

# 安装
将本仓库clone到`/root/.hydro/addons`目录下，进入仓库目录，运行：
```bash
yarn
```
后运行：
```bash
hydro addon add /root/hydro/addons/Hydro-Acrylic
```
即安装完毕。

安装后请重启Hydro以生效：
```bash
pm2 restart hydrooj
```

# 添加/修改背景图
在`frontend`目录下找到`nav-full.page.ts`，在第9行可填写url，格式如下：
```css
background-image: url("你的图片URL");
```
若要使用Base64格式存储图像以获得更好的使用体验，请更改为：
```css
background-image: url("data:image/png;base64,Base64数据");
```
Base64更改图片格式时须更改`data:image/`后的格式名。具体格式请自行百度CSS background-image格式。
