# 第三版：大笑奶龙

这一版把抽象感拉得更满：芥末黄梨形大肚子、奶白肚皮、深灰双手抱肚、细长粗腿，以及几乎占满脸的黑色大笑嘴。动作围绕“笑到失控”设计，同时保留 Codex 桌面宠物需要的完整状态与 16 向视线。

![待机动画预览](preview-idle.gif)

## 安装

1. 创建目录：

       %USERPROFILE%\.codex\pets\nailoong-laughing

2. 将本目录中的两个文件复制进去：

       pet.json
       spritesheet.webp

3. 编辑 `%USERPROFILE%\.codex\config.toml`，在已有的 `[desktop]` 段中设置：

       [desktop]
       selected-avatar-id = "custom:nailoong-laughing"

4. 若未立即生效，重启 Codex 桌面版。

## 文件

| 文件 | 说明 |
| --- | --- |
| `pet.json` | 第三版宠物元数据 |
| `spritesheet.webp` | 可直接安装的 8×11、RGBA v2 图集 |
| `preview-idle.gif` | 待机动画预览 |
| `contact-sheet.png` | 全部动作与视线帧总览 |
| `look-directions.png` | 16 向视线专项预览 |
| `validation.json` | 最终机器验证结果 |
| `direction-blind-validation.json` | 三轮独立方向盲测汇总 |
| `direction-semantics.json` | 16 个视线方向的语义复核 |
| `look-continuity.json` | 相邻视线帧连续性测量 |

图集机器校验结果：1536×2288、WebP/RGBA、8×11、`spriteVersionNumber = 2`，无格式、透明度或色键错误。方向盲测的硬门槛全部通过；一组细微斜角差异记录为已人工复核的 warning。

## 说明

这是非官方、粉丝创作的 AI 辅助衍生包。第三方角色、名称、形象和商标权利不包含在仓库的代码/文档许可中；详见仓库根目录的 [`NOTICE.md`](../NOTICE.md) 与 [`LICENSE-CODE`](../LICENSE-CODE)。
