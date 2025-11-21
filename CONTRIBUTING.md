# 贡献指南

首先，感谢你对 EnglishWords 项目的关注和支持！🎉

本文档将指导你如何有效地为这个项目做出贡献。

---

## 目录

- [行为准则](#行为准则)
- [如何贡献](#如何贡献)
- [开发环境设置](#开发环境设置)
- [代码规范](#代码规范)
- [提交PR流程](#提交pr流程)
- [报告Bug](#报告bug)
- [功能建议](#功能建议)

---

## 行为准则

### 我们的承诺

为了营造一个开放和热情的社区，我们承诺：

- 对所有人保持尊重和包容
- 欢迎不同的观点和经验
- 接受建设性的批评
- 专注于对社区最好的事情

### 不可接受的行为

以下行为不可接受：

- 使用带有性暗示的语言或图像
- 人身攻击、诋毁或嘲笑
- 骚扰或不尊重的评论
- 任何非法或有害的行为

如遇到不当行为，请邮件举报。

---

## 如何贡献

### 贡献的方式

1. **报告Bug** - 帮助我们识别和修复问题
2. **建议功能** - 提出改进和新功能想法
3. **编写代码** - 提交代码改进或新功能
4. **改进文档** - 完善项目文档
5. **扩展词库** - 添加更多单词和相关信息
6. **测试** - 测试功能并报告问题

---

## 开发环境设置

### 前置要求

- Git
- Node.js 18+ (如开发前后端)
- Python 3.9+ (如使用Python后端)
- Docker & Docker Compose (可选，推荐)

### 克隆仓库

```bash
git clone https://github.com/heiyijiushi/EnglishWords.git
cd EnglishWords
```

### 创建功能分支

```bash
git checkout -b feature/your-feature-name
# 或修复bug
git checkout -b fix/your-bug-fix

# 分支命名规范：
# feature/* - 新功能
# fix/* - bug修复
# docs/* - 文档更新
# test/* - 测试
# refactor/* - 代码重构
# perf/* - 性能优化
```

### 后端开发环境

#### 使用Nest.js (推荐)

```bash
cd backend
npm install
npm run dev
# 访问 http://localhost:3000
```

#### 使用FastAPI (Python)

```bash
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
python main.py
# 访问 http://localhost:8000
```

### 前端开发环境

```bash
cd frontend
npm install
npm run dev
# 访问 http://localhost:5173 (Vite默认端口)
```

### Docker开发

```bash
docker-compose up
# 自动启动所有服务
```

---

## 代码规范

### 通用规范

- **命名**：使用英文，避免拼音和中英文混合
- **注释**：英文注释，简明扼要
- **提交**：原子性提交，一次一个逻辑改动
- **行长**：建议不超过100个字符

### JavaScript/TypeScript

```typescript
// ✅ 好的例子
const getUserById = (userId: string): Promise<User> => {
  return api.get(`/users/${userId}`);
};

// ❌ 避免
const getUser = (id) => {
  return api.get('/users/' + id);
};
```

**规范工具：**
- ESLint - 代码质量检查
- Prettier - 代码格式化
- TypeScript - 类型检查

**运行检查：**
```bash
npm run lint
npm run format
npm run type-check
```

### Python

```python
# ✅ 好的例子
async def get_user(user_id: str) -> User:
    return await db.get_user(user_id)

# ❌ 避免
def get_user(id):
    return db.get_user(id)
```

**规范工具：**
- Black - 代码格式化
- Flake8 - 代码质量检查
- mypy - 类型检查

### 提交消息规范

使用 Conventional Commits 格式：

```
<type>(<scope>): <subject>

<body>

<footer>
```

**类型（type）：**
- `feat` - 新功能
- `fix` - bug修复
- `docs` - 文档修改
- `style` - 格式变更（不影响代码逻辑）
- `refactor` - 代码重构
- `test` - 添加或修改测试
- `chore` - 构建、依赖等修改

**示例：**

```
feat(auth): add JWT token refresh mechanism

- Implement refresh token endpoint
- Update token validation middleware
- Add token expiration handling

Fixes #123
```

---

## 提交PR流程

### 1. 提交前检查

- [ ] 代码通过本地测试
- [ ] 运行了linter和formatter
- [ ] 添加了必要的测试
- [ ] 更新了相关文档
- [ ] 提交消息遵循规范

### 2. 创建Pull Request

```bash
# 推送分支
git push origin feature/your-feature-name

# 在GitHub上创建PR
# - 标题清晰
# - 描述包含改动内容
# - 关联相关Issue（使用 Fixes #123）
# - 添加标签（如 enhancement, bug fix等）
```

### 3. PR描述模板

```markdown
## 描述
简要描述此PR的改动。

## 改动类型
- [ ] Bug修复
- [ ] 新功能
- [ ] 文档更新
- [ ] 代码重构
- [ ] 性能优化

## 改动详情
详细说明改动内容、原因和方式。

## 测试
描述如何测试这些改动。

## 相关Issue
Fixes #123

## 检查清单
- [ ] 代码遵循项目规范
- [ ] 添加/更新了相关文档
- [ ] 添加了必要的测试
- [ ] 所有测试都通过了
- [ ] 无breaking changes（如有，已在描述中说明）
```

### 4. 代码审查

- 维护者会在1-3天内审查你的PR
- 可能会要求修改或提出建议
- 一旦批准，维护者会合并你的代码

---

## 报告Bug

### 创建Bug报告

在GitHub Issues中：

1. **使用清晰的标题**：描述具体问题，而不是"Something is wrong"
2. **提供详细的步骤**：列出重现bug的确切步骤
3. **提供示例**：包含代码示例、错误消息或截图
4. **描述观察结果**：实际发生了什么
5. **描述预期结果**：你认为应该发生什么
6. **提供环境信息**：操作系统、浏览器版本、Node.js版本等

### Bug报告模板

```markdown
## Bug描述
清晰简洁的bug描述。

## 重现步骤
1. 步骤1
2. 步骤2
3. ...
4. 看到错误

## 预期行为
应该发生什么。

## 实际行为
实际发生了什么。

## 错误信息
[如果有，粘贴完整的错误堆栈]

## 环境
- 操作系统：
- Node.js版本：
- npm/yarn版本：
- 浏览器版本：

## 额外信息
任何其他相关信息。
```

---

## 功能建议

### 创建功能请求

1. **使用清晰的标题**：简洁地描述功能
2. **提供详细描述**：
   - 这个功能解决什么问题？
   - 期望的行为是什么？
   - 有没有替代方案？
3. **提供上下文**：为什么这个功能对你很重要？
4. **添加示例**：如果可能，提供具体的例子

### 功能请求模板

```markdown
## 功能描述
清晰地描述你想要的功能。

## 解决的问题
这个功能会解决什么问题？

## 建议的解决方案
你认为应该如何实现这个功能？

## 替代方案
考虑过哪些替代解决方案？

## 额外上下文
其他背景信息。
```

---

## 代码审查检查清单

审查PR时，我们会检查：

### 功能性
- [ ] 代码是否按预期工作？
- [ ] 是否处理了边界情况？
- [ ] 是否有明显的bug或逻辑错误？

### 代码质量
- [ ] 代码是否遵循项目规范？
- [ ] 变量和函数名是否清晰？
- [ ] 是否存在不必要的复杂性？
- [ ] 是否有机会进行重构？

### 测试
- [ ] 是否添加了足够的测试？
- [ ] 所有测试都通过了吗？
- [ ] 测试是否涵盖了主要场景？

### 文档
- [ ] 是否更新了相关文档？
- [ ] 是否添加了注释解释复杂逻辑？
- [ ] API改动是否在文档中记录？

### 性能
- [ ] 是否引入了性能问题？
- [ ] 是否可以优化？

### 安全性
- [ ] 是否处理了用户输入？
- [ ] 是否有潜在的安全漏洞？

---

## 获取帮助

- 📖 查看[项目文档](./README.md)
- 🗺️ 查看[开发路线图](./DEVELOPMENT_ROADMAP.md)
- 💬 在[GitHub Discussions](../../discussions)中提问
- 📝 查看相关[Issues](../../issues)中的讨论

---

## 许可证

通过贡献代码，你同意你的贡献将在项目的许可证（MIT）下发布。

---

## 致谢

感谢所有为EnglishWords做出贡献的开发者！🙌

---

*最后更新：2024年*

*版本：v1.0*
