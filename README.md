# multi-social

一个用于中英文视频内容的全平台分发 Codex skill：将明确指定的素材包分发到抖音、小红书（Red Note）、B站、X、TikTok、YouTube、Instagram、LinkedIn 和 Facebook。

它会帮助你锁定素材与封面、适配各平台文案、准备审核，并在每个平台记录真实的提交与发布状态；不会因为调用 skill 而自动发布内容。

## 安装

下载或克隆本仓库后，把整个目录复制到你的 Codex skills 目录：

```bash
git clone https://github.com/chenkan0617chris/multi-social.git
mkdir -p ~/.codex/skills
cp -R multi-social ~/.codex/skills/multi-social
```

重启或重新加载 Codex 后，即可使用：

```text
$multi-social 用 /绝对路径/素材包，准备九个平台，先不要发布。
```

## 使用示例

```text
$multi-social 只准备这个包的英文版到 X、TikTok 和 YouTube Shorts。
$multi-social 继续这个包，只处理还没完成的平台。
```

默认是“上传、填好、待审核”。只有在用户明确要求直接发布时，才会提交当次指定的内容。

## 许可证

本项目采用 [MIT License](LICENSE)。
