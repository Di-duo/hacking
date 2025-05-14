# 嘛？

一个强大的 Google Hacking 搜索工具，支持多搜索引擎（百度、Google、必应）的信息收集。

## 功能介绍

- 多搜索引擎支持：
  - 百度搜索
  - Google 搜索
  - 必应搜索
- 自动生成 Google hacking查询语法
- 自动处理长查询语句（百度好像是只允许 35 汉字内还是嘛，一下子忘了。查询百度的时候会处理语法长度）
- 实时显示搜索结果数量（这个不准，能力有限，慢慢改进）

- 20250514更新版本 v1.1：
  - 报告不再生成 txt
  - 生成html报告
  <img width="1415" alt="image" src="https://github.com/user-attachments/assets/bb763397-7490-4625-a483-c3b95901f0a3" />

## 工具使用截图
<img width="1012" alt="image" src="https://github.com/user-attachments/assets/e7c700d2-4902-46ef-8999-b6e7d8af158b" />
<img width="1020" alt="image" src="https://github.com/user-attachments/assets/82b9875c-472e-4370-94db-e0cfbe26980d" />
<img width="1022" alt="image" src="https://github.com/user-attachments/assets/df5bb5ef-ccad-4867-958e-b6cbd2f54240" />

## 内置语法

排查敏感字段：

site:*、*(password)

排查敏感文件：

Xls：filetype:xls site:*、*

PDF：filetype:pdf site:*、*

Word：filetype:doc site:*、*

排查黑客常用站点pastebin：

Site:pastebin.com.cn "&" | "&" | "&" | "&"

排查Github代码泄露情况：

site:github.com text:"&" | "&" | "&" | "&"

泄漏文件排查：

Sql文件：site:*、* ext:sql

site:github.com ext:sql github.com ext:sql "&" | "&" | "&" | "&"

TXT：Site:*、*:txt

Word：Site:*、*:doc

PDF：Site:*、*:pdf

排查敏感字段：

字段Password：Site:*、* intext:password

字段admin：Site:*、* intext:admin

排查代码托管bitbucket：

site:bitbucket.org+ "&" | "&" | "&" | "&"

排查gitlab：

site:gitlab.com+ "&" | "&" | "&" | "&"

排查sorceforge：

site:sorceforge.net+ "&" | "&" | "&" | "&"

排查码云：

site:gitee.com+ "&" | "&" | "&" | "&"

阿里云Code：

site:code.aliyun.com+ "&" | "&" | "&" | "&"

码市：

site:coding.net+ "&" | "&" | "&" | "&"

腾讯云dev：

site:dev.tencent.com+ "&" | "&" | "&" | "&"

site:dev.tencent.com("&" | "&" | "&" | "&")

CSDN CODE：

site:code.csdn.net+ "&" | "&" | "&" | "&"

百度效率云：

site:xiaolvyun.baidu.com+ "&" | "&" | "&" | "&"

SVNChina:

site:SVNChina:.com+ "&" | "&" | "&" | "&"

SVNBucket:

Site:SVNBucket.com("&" | "&" | "&" | "&")

Alisvn：

site:Alisvn.com("&" | "&" | "&" | "&")

Daocloud：

site:hub.docker.com("&" | "&" | "&" | "&")
