# FIRE 倒计时

4% 法则：年支出 × 25 = 财务自由目标——算算还有几年

> 点子来源：Obsidian《人生可视化 / FIRE 倒计时》 · 同系列仓库参考 [life-grid](https://github.com/palmyer/life-grid)

## 功能

- 目标金额与进度条
- 逐年复利模拟：按当前储蓄速度的达成年份与年龄
- 里程碑：25% / 50% / Coast FIRE / 财务自由

## 运行

纯静态零依赖，任选其一：

```bash
cd fire-countdown
python -m http.server 8740
```

- 网页版：<http://127.0.0.1:8740/>
- 手机壳预览：<http://127.0.0.1:8740/preview.html>（life-grid 同款）

或直接双击 `index.html`。

## 设计

- iOS 暗色风格：纯黑背景、#1C1C1E 分组卡片、SF 系统色板
- 选择一律使用 iOS 风格底部滚轮（`shared/wheel.js`）
- 数据存于浏览器 localStorage（`lv-` 前缀），不上传任何服务器
- 生日 / 预期寿命与同系列工具共享同一份配置
