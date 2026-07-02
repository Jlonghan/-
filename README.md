# claude-short-video-script

全行业通用短视频脚本生成器 — Claude Code Skill

一句话输入 → 完整短视频脚本直接可拍。支持任意行业、任意人设、任意产品/服务。

---

## 功能

- **首次使用**：自动引导填写 10 个问题，完成你的行业人设配置
- **配置后**：一句话输入话题方向，直接生成 300-400 字可拍脚本
- **支持 4 大内容方向**：解决难题 / 案例引入 / 推荐建议 / 揭秘避坑
- **内置爆款元素**：8 大爆款元素、钩子库、爆词库、热门公式全套
- **多人设支持**：最多两个人设，各自语气风格独立

---

## 安装

### 方法一：直接复制文件

把 `skill/` 目录里的文件复制到你的 Claude Code skills 目录：

```bash
# 创建 skill 目录
mkdir -p ~/.claude/skills/short-video-script

# 复制文件
cp skill/SKILL.md ~/.claude/skills/short-video-script/SKILL.md
cp skill/profile-template.md ~/.claude/skills/short-video-script/profile-template.md
```

### 方法二：直接克隆

```bash
git clone https://github.com/Jlonghan/claude-short-video-script.git
mkdir -p ~/.claude/skills/short-video-script
cp claude-short-video-script/skill/SKILL.md ~/.claude/skills/short-video-script/SKILL.md
cp claude-short-video-script/skill/profile-template.md ~/.claude/skills/short-video-script/profile-template.md
```

---

## 使用方法

安装后，在 Claude Code 中输入：

```
/short-video-script
```

**首次使用**会自动进入配置向导，回答 10 个问题后配置保存到本地，以后直接用。

**日常使用示例：**

```
/short-video-script 做一条关于客户踩坑的视频
/short-video-script 写一个案例引入的脚本 persona:人设A
/short-video-script 给我出揭秘类的文案
```

**修改配置：**

```
/short-video-script 更新配置
```

---

## 目录结构

```
claude-short-video-script/
├── README.md
└── skill/
    ├── SKILL.md              # 主 skill 文件
    └── profile-template.md   # 用户配置模板（可手动填写替代向导）
```

---

## 手动配置（可选）

不想走配置向导？把 `skill/profile-template.md` 里的内容复制出来，填写你自己的信息，保存为：

```
~/.claude/skills/short-video-script/profile.md
```

下次运行 `/short-video-script` 会自动加载，跳过向导。

---

## 核心内容方向

| 方向 | 文案结构 |
|------|---------|
| 解决难题 | 场景难题 → 放大危机 → 低成本解决 → 具体操作 |
| 案例引入 | 案例描述 → 提取知识点 → 用户应对方法 |
| 推荐建议 | 美好愿景 → 圈定人群 → 引发好奇 → 推荐理由 |
| 揭秘避坑 | 提出揭秘事件 → 讲述内情 → 如何避免 |

---

## License

MIT
