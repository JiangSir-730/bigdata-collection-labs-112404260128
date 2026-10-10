# GitHub 实验提交说明

> 本说明主要用于第一次实验。后续实验继续使用同一个课程仓库。

# 1. 创建课程仓库

仓库名称统一为：

```text
bigdata-collection-labs-学号
```

例如学号为 `2026123456`：

```text
bigdata-collection-labs-2026123456
```

建议设置为 **Private**。

如教师要求添加 Collaborator 或使用 GitHub Classroom，按课堂通知执行。

---

# 2. 仓库首页写明学生信息

仓库根目录建立 `README.md`：

```markdown
# 大数据采集与处理实验

- 姓名：张三
- 学号：2026123456
- 班级：数据科学与大数据技术XX班
```

`lab01/REPORT.md` 开头也必须填写：

```text
姓名
学号
班级
GitHub 用户名
仓库地址
```

---

# 3. Lab 1 最终目录

```text
bigdata-collection-labs-2026123456/
├── README.md
└── lab01/
    ├── lab1_html_api.ipynb
    ├── REPORT.md
    ├── data/
    │   ├── companies.json
    │   └── devices.json
    └── images/
        ├── 01_device_api.png
        ├── 02_company_source.png
        ├── 03_company_next.png
        └── 04_validation.png
```

4 张截图含义固定：

```text
01_device_api.png
→ 浏览器 DevTools / Network
→ 设备 Fetch/XHR 请求 + Request URL + 分页参数

02_company_source.png
→ “查看网页源代码”
→ Ctrl+F 搜索真实企业名称并能找到

03_company_next.png
→ 浏览器 DevTools / Elements
→ 选中“下一页”对应的 <a> 元素并看清 href

04_validation.png
→ JupyterLab 运行结果
→ 60 / 60 / 5000 / 5000 / mismatch 等最终验证数字
```

不要用代码截图代替上述证据图。

---

# 4. 第一次使用 Git

```bash
git clone https://github.com/你的用户名/bigdata-collection-labs-你的学号.git
cd bigdata-collection-labs-你的学号
```

实验完成并整理文件后：

```bash
git status
git add .
git commit -m "Complete Lab 1 - 学号 姓名"
git push
```

例如：

```bash
git commit -m "Complete Lab 1 - 2026123456 张三"
```

本实验只要求掌握：

```text
git status
git add
git commit
git push
```

---

# 5. 提交前检查

先在 JupyterLab：

```text
Restart Kernel → Run All
```

再检查 GitHub：

```text
□ 仓库名中有自己的学号
□ README.md 有姓名、学号、班级
□ lab01/lab1_html_api.ipynb
□ lab01/REPORT.md
□ lab01/data/companies.json
□ lab01/data/devices.json
□ lab01/images/ 下有规定的 4 张截图
□ REPORT.md 中 4 张图片都能正常显示
□ REPORT.md 中关键代码空格已填写
□ GitHub 中能够看到本次实验 commit
```

---

# 6. 学习通提交

**学习通只提交 GitHub 仓库链接。**

例如：

```text
https://github.com/yourname/bigdata-collection-labs-2026123456
```

不需要重复上传 Notebook、REPORT、JSON 或截图。
