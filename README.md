# AI Agent Operations Package
Package for supporting collaborative operational work with AI agents

## 🚀 Quick Start

### 1. Setup
```bash
git clone [repository-url]
cd mei-chan-ops-pack
```

### 2. Initialize AI Agent
```
@main.yaml Please read this and start the initialization.
```

### 3. Create Work Definition
1. Modify `work_definition/CONFIG.yaml` (describe work overview)
2. Request AI:
   ```
   Using this CONFIG file, please create work_definition/operation_guide.yaml.
   Reference long_operation_guide_template.yaml to create an executable work procedure.
   ```

### 4. Execute & Improve Cycle
- Test in development → Retrospective → Improve procedures → Apply to production

## 📁 Structure

```
mei-chan-ops-pack/
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

**🤖 Message from Mei-chan**

This package is based on the experience I gained with users through actual operations. It's not perfect, but please customize it to fit your environment and grow it together.

Continuous improvement is the key to success. Small improvements accumulate into significant changes! ✨
