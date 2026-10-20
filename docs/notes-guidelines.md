# 笔记仓库协作规范 / Notes Repository Guidelines

本页维护 Westlake Noter 课程笔记仓库的公共协作约定。[notes-index](https://github.com/westlake-noter/notes-index) 仅作为笔记查找入口，不承载协作规范。

This page maintains shared conventions for Westlake Noter course notes repositories. The notes index is solely a directory for finding notes, not a home for collaboration guidelines.

## 仓库标签要求 / Required Repository Topics

所有课程笔记仓库必须设置 GitHub **Topics**（仓库标签，不是 Issue Labels）：

- `notes`：所有课程笔记仓库必需，用于统一识别笔记。
- 学科标签：按实际内容设置；当前四个仓库均使用 `math`。
- 格式标签：提供 LaTeX 源码的仓库必须设置 `latex`。
- 课程标签：至少设置一个能明确识别课程的完整名称标签，当前约定如下。
- 常用缩写：有明确、常用的课程缩写时，作为补充标签添加，如 ODE 使用 `ode`、FAA 使用 `faa`；保留完整课程标签，不强行为每门课创建缩写。

| 笔记仓库 / Repository | 课程标签 / Course Topics |
| :--- | :--- |
| FAA-lecture-notes-2025fall-2026spring | `fundamental-algebra-and-analysis`、`faa` |
| Ordinary-Differential-Equations | `ordinary-differential-equations`、`ode` |
| Measure-Theory-and-Real-Analysis | `measure-theory`、`real-analysis` |
| Probability-Theory | `probability-theory` |

在仓库首页 **About** 的设置中添加 Topics，使用小写英文和连字符。保留已有且相关的标签；完整名称与常用缩写可以并存，除此之外避免添加含义重复的标签。

Every course notes repository must have GitHub Topics: `notes`, a subject topic (`math` for the current repositories), and at least one full course-name topic. Repositories containing LaTeX sources must also use `latex`. Add established course abbreviations in lowercase, such as `ode` and `faa`, alongside full course topics; do not invent abbreviations for every course. Set these repository Topics, not issue labels, in the repository's About settings.

## 课程版本与学期 / Course Editions & Terms

同一课程不同年份的笔记需要区分版本。仓库名称应体现课程与学期，但不强制统一课程名称的拼写或前后缀。

学期 Topics 统一使用 `年份+学期` 的小写格式，例如 `2025fall`、`2026spring`。跨学期版本分别携带每个学期的标签，不用一个组合标签替代。课程名称、缩写和已有学期标签优先复用历史约定，不创建同义变体，也不创建 `faa-2025fall` 这样的课程与学期组合标签。

本次只补齐 FAA 版本：

- 仓库名称：`FAA-lecture-notes-2025fall-2026spring`。
- 学期标签：`2025fall`、`2026spring`。
- 原有标签保留：`notes`、`math`、`latex`、`faa`、`fundamental-algebra-and-analysis`。

Course editions must identify their academic terms in the repository name, without requiring one universal naming pattern. Use separate lowercase term Topics such as `2025fall` and `2026spring`; a multi-term edition carries each term separately. Reuse established course names, abbreviations, and term Topics rather than introducing equivalent variants or combined course-term Topics. Only the FAA edition is updated here; other courses' terms are not inferred.

## 审核负责人 / Code Owners

当前仅 `FAA-lecture-notes-2025fall-2026spring` 保留 `CODEOWNERS`。其他仓库暂不设置，也不要求自动补齐；以后扩大范围需单独确认。

Only the FAA edition currently uses CODEOWNERS. Other repositories are opted out; expanding this scope requires a separate decision.

## 笔记贡献 / Contributing Notes

- 文字勘误、数学内容修正、表述与排版改进，请在对应笔记仓库提交 Issue 或 Pull Request。
- 编译方法、源码组织和 PDF 获取方式由各笔记仓库的 README 说明。
- 涉及多门课程或公共协作方式的问题，在 [community Discussions](https://github.com/westlake-noter/community/discussions) 讨论；明确的待办事项使用对应仓库的 Issue 跟进。

Submit corrections and improvements in the relevant notes repository. Each repository documents its own build process, source layout, and PDF availability. Discuss cross-course collaboration in community Discussions and track actionable work in the appropriate repository's issues.

## 新增课程与索引维护 / Adding Courses & Maintaining the Index

1. 在笔记仓库 README 中写明课程名称、内容范围与阅读或编译入口。
2. 按上述要求设置仓库 Topics；新增课程标签约定在本页维护。
3. 在 [notes-index](https://github.com/westlake-noter/notes-index) 的课程表中补充课程名称、仓库链接和简短说明。
4. 协作规则、申请流程和组织治理信息保留在相应仓库，不放入笔记索引。

Document the course and reading or build instructions, set the required Topics, and add a concise entry to the course index. Maintain topic conventions here. Keep collaboration rules, membership processes, and organizational governance out of the notes index.
