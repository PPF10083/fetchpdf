---
name: fetchpdf
description: 按 DOI、PMID 或文献清单获取全文与补充材料
---

# 默认工作流

> 默认无需检查环境。

## 1. 下载文献

单篇论文可直接传入 DOI 或 PMID：

```bash
fetchpdf "10.1038/nature12373" -o ./papers --make-subfolder --on-existing supplement --get-xml-or-html --to-markdown
```

多篇论文需提供 CSV 文件。可参考 [DOI CSV 示例](reference/doi_template.csv) 或 [PMID CSV 示例](reference/pmid_template.csv)。DOI 清单使用 `--csv`，PMID 清单使用 `--pmid-csv`。命令如下：

```bash
fetchpdf /path/to/csv -o /path/to/download --make-subfolder --on-existing supplement --get-xml-or-html --to-markdown
```

多篇论文下载耗时较长，建议按以下方式检查进度：

1. 根据任务进展估算剩余耗时，合理安排检查间隔，避免无意义的重复检查；
2. 记录本次下载进程的 PID，通过进程状态判断是否结束。

查询 fetchpdf CLI 的用法：

```bash
fetchpdf --help
```

## 2. 联网搜索补齐未获取文献

1. 默认由具备联网搜索能力的轻量级子 Agent（如 Flash、Luna）查找可公开获取的全文与补充材料；不可用时由主 Agent 完成，并如实说明。
2. 结果须包含来源 URL、文献版本、身份核验依据，以及实际保存路径或未获取原因。仅找到候选链接不算获取成功。

### 多篇文献的获取结果更新（单篇文献跳过）

> 联网搜索补救结束后，同步更新输出目录中的 `failed_dois.csv` 和 `missing_pdfs.html`，记录实际获取结果。
> 仅在文件已保存且通过身份与格式验证后，才更新为成功；若仅有候选链接，则仍标记为未获取，并更新原因。
> 若仅获得 XML/HTML 全文，应注明“全文已获取，PDF 未获取”，避免将全文获取与 PDF 获取混为一谈。

## 3. 输出检查

`fetchpdf` 已在下载时完成文件校验，无需重复进行内容验证。