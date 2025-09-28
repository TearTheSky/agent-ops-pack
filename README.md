# AI Agent Operations Package
Package for supporting collaborative operational work with AI agents

## 🚀 Quick Start

### 1. Setup
```bash
git clone [repository-url]
cd agent-ops-pack
```

### 2. Initialize AI Agent
```
@main.yaml Please read this and start the initialization.
```

### 3. Create Work Definition
1. Modify `work_definition/CONFIG.yaml` (describe work overview)
2. Request AI:
   ```
   (Attach the modified CONFIG.yaml as reference material)
   Using this CONFIG, please create AI agent procedures by utilizing all available reference documents.

   【Important Constraints】
   - Do not reference non-existent files (fictional file names are prohibited)
   - Record unimplemented features as manual tasks
   - Prioritize practical procedures over incomplete but perfect ones
   - Clearly mark areas where AI judgment is uncertain as human confirmation points

   【Structuring Policy】
   - Extract components into subtasks and organize them in a modular structure
   - However, only reference files that are actually created

   【Environment-specific Handling】
   - Create environment-specific procedures referring to environment/system_environment.yaml
   - Manage environment-specific settings globally to avoid duplication
   - Record currently unknown environment differences as "to be discovered and added through future dialogue"

   【Quality Assurance】
   - Finally verify and correct file path consistency
   - Delete non-existent references or convert them to manual tasks
   ```

### 4. Quality Review Implementation
We strongly recommend that created procedures undergo rigorous review by AI agents:
```
Please review the created procedures from the perspective of an experienced senior engineer with practical experience, providing useful reviews.

【Document Nature】
- Personal AI operation procedures (not generic templates)
- Living documents that grow
- Practicality > Theoretical perfection

【Review Perspectives】
1. Practicality: Will this actually cause problems in real work?
2. Safety: Can it prevent serious accidents?
3. Maintainability: Can it be easily updated and improved?
4. Learning Cost: Are there too many new things to remember?

【Avoid These Types of Feedback】
- Unnecessary complication of working systems
- Excessive abstraction and framework-ization
- Solving problems that aren't actually causing issues
- Design changes for the sake of generalization
```

**Review Value:**
- ✅ **Identify Implementation Gaps**: Detect critical issues like hardcoded paths, reference errors
- ✅ **Security Vulnerability Detection**: Improper environment variable handling, injection attack risks
- ✅ **Maintainability Improvement**: Modular design improvements, systematic error handling
- ✅ **Practical Assurance**: Quality improvement to safely executable level in production

### 5. Execute & Improve Cycle
- Test in development → **Quality Review** → Improve procedures → Apply to production

## 📁 Structure

```
agent-ops-pack/
├── main.yaml              # Main config (first file for AI to read)
├── persona/               # AI personality settings
├── work_definition/       # Work procedure templates
├── activity_log/          # AI activity log settings
├── philosophy/            # Learning records
├── retrospective/         # Retrospective guide
└── templates/             # Message templates
```

## 💡 Features

- **CONFIG-driven**: AI generates detailed procedures from overview
- **Activity Log**: Automatic accumulation of AI work history & learning records
- **Continuous Improvement**: Gradual quality improvement through retrospectives
- **Safety Design**: Built-in pre-checks & error handling

## 🎯 Target Operations

- Infrastructure operations (Terraform, Kubernetes, etc.)
- Database operations (backup, maintenance, etc.)
- CI/CD operations (deployment, version upgrades, etc.)
- Incident response & recovery operations

## ⚠️ Important

- **Retrospective Required**: Must be conducted after work. Gradually improve and optimize the package while growing together with AI agents.
- **Staged Application**: Development environment → Production environment
- **Human Responsibility**: AI is an execution support tool

---

**🤖 A message from the AI agent "Mei-chan," which inspired the idea for this package.**

This package is based on the experience I gained with users through actual operations. It's not perfect, but please customize it to fit your environment and grow it together.

Continuous improvement is the key to success. Small improvements accumulate into significant changes! ✨
