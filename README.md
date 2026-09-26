# 美学技能库 · Aesthetic Skills

面向图像创作与视觉设计的中文美学技能集合。将创作规则、提示词模板和执行流程整理为独立的 `SKILL.md`，方便按需安装和持续改进。

## 技能目录

| 技能 | 用途 | 所需能力 |
| --- | --- | --- |
| [极简机器人头像](skills/minimal-robot-avatar/SKILL.md) | 将人物照片、插画或文字角色转为极简胶囊眼头像，支持局部修改 | 实际出图需要图像生成或编辑工具；仅编写提示词无需图像工具 |

## 安装

下载本仓库，或使用 Git 克隆：

```bash
git clone https://github.com/5Lee/aesthetic-skills.git
cd aesthetic-skills
```

将需要的技能文件夹复制到你的 Codex 技能目录。以下命令在下载后的仓库根目录执行，适用于 macOS / Linux：

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
# 如果目标位置已有同名技能，请先备份并比较，再决定是否替换。
cp -R skills/minimal-robot-avatar "${CODEX_HOME:-$HOME/.codex}/skills/"
```

也可以向支持安装技能的助手提供本仓库地址及技能路径 `skills/minimal-robot-avatar`。

技能提供工作方法和提示词，不自带图像模型、API 密钥或付费额度。使用其他支持 SKILL.md 的客户端时，应按该客户端的目录规则安装。

## 使用

附上目标照片，再发送：

> 使用 $minimal-robot-avatar，把这张照片转成极简机器人头像，保留发型和眼镜。

构图默认从左下探入，也支持居中、从右向左探入和自定义倾斜或视角。例如：“居中，头摆正”或“从右边探入，逆时针倾斜 25 度”。鼻子和嘴巴仍默认省略。

也支持纯文字创作：

> 使用 $minimal-robot-avatar，设计一个银白色脸、橙色短发、蓝色耳机的机器人头像。

只需要提示词时：

> 使用 $minimal-robot-avatar，帮我写提示词，先不要出图。

## 仓库结构

```text
skills/
  minimal-robot-avatar/
    SKILL.md
    agents/openai.yaml
    references/prompt-template.md
ATTRIBUTION.md
```

每个技能独立维护；仅复制需要的技能即可。新增技能时在 `skills/` 下创建独立目录，写清用途、依赖、使用示例，并更新目录表和来源记录。

## 验证状态

极简机器人头像技能已通过技能结构校验与内部引用检查，尚未进行实际图像生成测试。模型和工具不同，图像效果也可能不同。

## 来源与许可

请参阅 [ATTRIBUTION.md](ATTRIBUTION.md)。本仓库尚未授予统一的开源许可证；公开访问不等于获得任意转载、再许可或商业分发授权。后续可在确认各项内容的权利与授权后补充适用许可证。
