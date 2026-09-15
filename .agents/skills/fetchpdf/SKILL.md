---
name: fetchpdf
description: 按 DOI、PMID 或文献清单获取全文与补充材料
---

# 默认工作流

## 1. 下载文献

单篇论文直接传入 DOI 或 PMID：

```
fetchpdf "10.1038/nature12373" -o ./papers --make-subfolder --on-existing supplement --get-xml-or-html --to-markdown
```

多篇论文则需要 CSV 文件。CSV 文件参考：[DOI CSV 示例](reference/doi_template.csv) 或 [PMID CSV 示例](reference/pmid_template.csv) 。DOI 清单使用 `--csv`，PMID 清单使用 `--pmid-csv`。
多篇论文使用如下命令：

```
fetchpdf /path/to/csv -o /path/to/download --make-subfolder --on-existing supplement --get-xml-or-html --to-markdown
```

查询如何使用 fetchpdf cli：
```
fetchpdf --help
```

## 未获取样本

将未获取文献的 DOI、标题及失败原因交给具备联网搜索能力的子 Agent，优先使用 Flash、Luna 等轻量级模型，查找可公开获取的全文与补充材料。

# 文件检查

`fetchpdf` 会自动进行必要的检查，无需复查。

# 首次安装配置

如果你正在安装这个 SKILL, 阅读[环境配置](reference/config.md)。
