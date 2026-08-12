# 紫猫工作流目录

这是紫猫桌面软件使用的公开 ComfyUI 工作流目录。仓库只存放经过审核的小型工作流文件、资源清单和签名，不存放大模型。

## 当前工作流

- MiniMax H3 `260803`
- 文生视频、首帧/首尾帧、全能参考
- 最低 NVIDIA 8 GB 显存、16 GB 系统内存
- 模型来源：`Comfy-Org/MiniMax-H3`
- Hugging Face revision：`014cd40f7e177756c6b2473c0d93b1c89a790dd2`

## 软件读取地址

```text
https://raw.githubusercontent.com/xufeifei083-maker/zimao-workflows/main/catalog/catalog.json?v=260803-1
```

签名文件位于同地址的 `catalog.json.sig`，公钥见 [`public-key.txt`](public-key.txt)。软件必须先验证 Ed25519 签名，再接受目录内容；每个模型还会验证完整 commit、文件大小和 SHA256。

## 目录结构

```text
catalog/
  catalog.json
  catalog.json.sig
  workflows/<id>/<version>/*.json
public-key.txt
```

目录签名私钥不进入 GitHub，仅保存在发布机器的受保护目录中。
