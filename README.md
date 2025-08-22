# AI Agent Operations Package
## Package for Supporting Collaborative Work between AI Agents and Humans

### 📖 About This Package

This package is a **collection of tools for AI agents (ChatGPT, Claude, Gemini, etc.) and humans to collaborate safely and efficiently in operational tasks**.

**We provide step-by-step explanations so that even those with limited understanding of AI can use it with confidence.**

## 🤖 What is an AI Agent?

**AI agents** are conversational AIs like ChatGPT, Claude, Gemini, etc.

### Characteristics of AI Agents
- ✅ **Can work 24/7** (humans need breaks)
- ✅ **Can process large amounts of information quickly**
- ✅ **Not influenced by emotions**
- ✅ **Can execute actual work if proper definitions are provided**
- ❌ **May not understand context sometimes**
- ❌ **Cannot take responsibility** (humans have final responsibility)

### Why Collaborate with AI Agents?
- **Efficiency**: Automate repetitive tasks
- **Quality Improvement**: Reduce human errors
- **Knowledge Sharing**: Improve team-wide skills
- **Continuous Improvement**: Optimize work processes

## 📁 Package Structure

```
mei-chan-ops-pack/
├── main.yaml                    # Main configuration file
├── persona/                     # AI agent personality settings
├── work_definition/            # Work procedure template
├── progress_tracking/          # Progress management system
├── philosophy/                 # Lessons learned and improvements
├── retrospective/              # How to conduct retrospectives
└── templates/                  # Message templates
```

## 🚀 How to Use (For Beginners)

### Step 1: Download the Package
```bash
# Clone or download this repository
git clone [repository-url]
cd mei-chan-ops-pack
```

### Step 2: Configure AI Agent Personality
1. Open `persona/ai_persona_template.yaml`
2. Modify settings to fit your team
3. Pay special attention to the "Recommended Change Zone" section

### Step 3: Give Personality to AI Agent and Explain Situation and Next Steps

**💡 Importance of This Step**
This step is crucial for building trust between AI agents and humans and establishing the foundation for effective collaborative work. AI agents start with no knowledge, so it's necessary to gradually deepen understanding over time.

**AI agents, like humans, are not perfect from the beginning. Let's learn and improve together.**

**🤝 Tips for Success**
- **Don't rush**: Explain according to the AI agent's level of understanding
- **Be specific**: Avoid abstract expressions, include concrete examples
- **Step by step**: Provide information progressively from basic to detailed
- **Feedback**: Actively respond to AI agent's questions and suggestions

```
"Please read the content of persona/ai_persona_template.yaml and help me with work using this personality.
Please read main.yaml first to understand the overall structure.

Please tell me what information is needed to create a work procedure for my project.
Don't make assumptions, ask for all necessary information.
It's not a sin for an AI who just started chatting to be ignorant. Please ask anything.

Especially the following information is needed:
- Tools to use (Terraform, GitHub, Slack, etc.)
- Specific commands and scripts
- File paths and working directories
- Permission and authentication methods
- Location of existing work procedures and scripts

After that, please provide specific suggestions for proceeding to Step 4 work procedure creation.
The recommendation is the method of 'modifying CONFIG.yaml to create initial version with AI auto-generation, testing in development environment, and growing together through retrospectives.'"
```

### Step 4: Create Work Procedure (Two Methods)

**💡 Importance of This Step**
Work procedures are the foundation for AI agents and humans to collaborate safely and efficiently. **It's impossible to create perfect procedures from the beginning**. It's important to have humans review and modify the initial version created by AI, test it in safe environments like development, and gradually upgrade through retrospectives while improving.

**🔄 Continuous Improvement Process**
1. **Human CONFIG.yaml modification (summary creation)**
2. **AI detailed elaboration (operation_guide.yaml creation)**
3. **Human review and modification**
4. **Testing in development environment**
5. **Identifying improvements in retrospectives**
6. **Work procedure version upgrade**
7. **Application in production environment**

#### Method A: Create Manually
1. Copy `work_definition/long_operation_guide_template.yaml`
2. Customize for your project
3. **Enter specific work procedures that AI agents can actually execute**

#### Method B: Have AI Auto-Generate (Recommended)
1. **Modify CONFIG file (Human performs)**
   - Modify the example in `work_definition/CONFIG.yaml` to fit your operational work
   - You can also add new parameters as needed
   - **CONFIG.yaml functions as a summary (overview) of the work**

2. **Request from AI Agent**
   ```
   "Please use this CONFIG file to create a new operation_guide.yaml in work_definition.
   Please refer to long_operation_guide_template.yaml to create a specific work procedure for my project.
   
   Please elaborate the summary (overview) in CONFIG.yaml and create an executable work procedure.
   
   Please include the following points:
   - Work start and completion recording
   - Communication app notification procedures (Slack, etc.)
   - Progress recording methods
   - Error communication methods
   - Retrospective implementation timing
   - Specific execution procedures for each task
   ```

3. **Review and adjust generated operation_guide.yaml**
   - **Refer to progress_tracking/progress_tracking_config.yaml** to confirm and adjust progress recording settings
   - **Refer to templates/slack_message_templates.yaml** to adjust notification messages
   - **Refer to retrospective/retrospective_how_to.yaml** to confirm retrospective procedures
   - Safety confirmation
   - Addition of project-specific requirements
   - Error handling confirmation
   - Detailed execution procedures for each task
   - **Confirm that CONFIG.yaml summary is appropriately detailed**

### Step 5: Actually Try It
- **Start work**: Request work from AI agent
- **Progress confirmation**: Regularly check status
- **Result recording**: Record progress after work completion
- **Team communication**: Report results on Slack
- **Retrospective implementation**: **Always conduct retrospectives!** No matter how little content or short, conduct retrospectives for continuous improvement!
- **Next improvement**: Apply learned lessons to next time

## 💡 Frequently Asked Questions (FAQ)

### Q: Are AI agents safe?
**A**: AI agents can not only **propose and support** but also **execute actual work if proper definitions and workflows are provided**. This package aims to share safe work procedures and executable definitions. For actual work, please use with appropriate additions and modifications under your own responsibility.

### Q: Can I use it without technical knowledge of AI?
**A**: Yes! This package is **explained step by step**, so you can use it even without AI knowledge. However, to control AI behavior when needed, you need to deepen your technical understanding of the system operations and development-related work you are responsible for.

### Q: Which AI agent should I use?
**A**: Please use AI integrated in your IDE. (Cursor, VS Code, IntelliJ IDEA, etc.) For AI in IDE, you can use any conversational AI model like ChatGPT, Claude, Gemini, etc. Please choose your preferred one.

### Q: Is customization necessary?
**A**: You can use basic settings as is, but we recommend **adjusting to your project**.

### Q: Are retrospectives really necessary?
**A**: **Absolutely necessary!** No matter how little content or short, conduct retrospectives! Retrospectives are essential for continuous improvement.

### Q: Creating operation_guide seems difficult...
**A**: We recommend the **method of modifying `work_definition/CONFIG.yaml` and requesting AI**. Humans just need to modify the CONFIG file example to fit their work, and AI will auto-generate `work_definition/operation_guide.yaml`. By referring to each configuration file for adjustment, you can create better work procedures.

## 📋 Role of Each File

### 🤖 `persona/` - AI Agent Personality Settings
**Purpose**: Set "what kind of personality you want the AI agent to work with"
- **Recommended Change Zone**: Must be changed to fit your team
- **Optional Change Zone**: Adjust as needed
- **Company Culture Consideration**: Language and communication style

### 📝 `work_definition/` - Work Procedure Template
**Purpose**: Define specific work procedures that AI agents can actually execute
- **CONFIG.yaml**: Define work overview and task structure
- **long_operation_guide_template.yaml**: Generic work procedure template
- **operation_guide.yaml**: Specific work procedure (auto-generated by AI)
- **Progressive execution**: Safely proceed with work
- **Error handling**: What to do when problems occur
- **Time measurement**: Record work time
- **Pre-execution checks**: Pre-evaluate risks
- **Executable commands**: Specific procedures that AI agents can actually execute
- **CONFIG-based generation**: AI auto-generates just by humans writing CONFIG
- **Communication and recording**: Slack notifications, progress recording, retrospective procedures included

### 📊 `progress_tracking/` - Progress Management System
**Purpose**: Record work progress and results
- **For spreadsheets**: Records for team sharing
- **AI work logs**: AI agent's own records
- **Evidence reports**: Records for issue tracking

### 📚 `philosophy/` - Lessons Learned and Improvements
**Purpose**: Record and share what was learned from work
- **Simple structure**: 3 items of problem, action, learning
- **Concrete examples**: Actual problems and solutions
- **Continuous improvement**: How to apply to next time

### 🔄 `retrospective/` - How to Conduct Retrospectives
**Purpose**: AI agents and humans conduct effective retrospectives
- **Basic principles**: Easy to understand design
- **5-step process**: Progressive retrospectives
- **Concrete examples**: Actual retrospective examples
- **Mandatory implementation**: **No matter how little content or short, always conduct retrospectives!**

### 📄 `templates/` - Message Templates
**Purpose**: Unified communication
- **Slack posts**: Team notifications
- **PR descriptions**: Unified format
- **Evidence reports**: For issue tracking

## 🎯 What Tasks Can It Be Used For?

### Infrastructure and Operations
- **Infrastructure operations and SRE**: Server management, monitoring setup, team communication
- **Database operations**: Backup, performance tuning, progress recording
- **Security operations**: Vulnerability response, access management, emergency communication
- **Monitoring and alert operations**: Alert setup, incident response, status reporting

### Development
- **Application development**: Deploy, test, review requests
- **CI/CD operations**: Pipeline construction, automation, result notifications
- **Version upgrade work**: Dependency updates, compatibility confirmation, change notifications

### Others
- **Incident response and recovery work**: Emergency response procedures, status reporting, retrospectives
- **Regular maintenance**: Planned maintenance work, progress management, completion reporting
- **Documentation creation**: Procedure creation, report creation, sharing and updates

## ✨ Features of This Package

### 🚀 Efficiency
- **Optimized for collaborative work between AI agents and humans**
- **Progressive execution** to safely proceed with work
- **Automation** to efficiently handle repetitive tasks

### 🛡️ Safety
- **Pre-execution checks** to evaluate risks
- **Error handling** to address problems
- **Safe work** even in production environments

### 📈 Continuous Improvement
- **Improve problems through retrospectives** (**mandatory implementation!**)
- **Record and share lessons learned**
- **Optimize work processes**
- **No matter how little content or short, always conduct retrospectives!**

### 🌍 Versatility
- **Generic design that can be used in any company**
- **Customizable** for flexible response
- **Progressive introduction** to start without pressure

## ⚠️ Important Notes

### 🔒 Security
- **AI can execute work if proper definitions and workflows are provided** (not just proposals and support, but actual work execution)
- **Don't include confidential information** (don't include in package)
- **Manage access permissions appropriately** (minimum necessary permissions)

### 📋 Operations
- **Always conduct retrospectives** (for continuous improvement)
- **No matter how little content or short, conduct retrospectives!**
- **Share and utilize across the entire team** (knowledge accumulation)
- **Customize to fit your project** (optimization)

### 🤖 Collaboration with AI Agents
- **Prepare appropriate definitions and workflows** (so AI can actually execute work)
- **Don't blindly trust AI responses** (always confirm and verify)
- **Humans take responsibility** (AI is a support tool but can execute actual work)
- **Continuously learn and improve** (both AI and humans grow)
- **Always conduct retrospectives** (no matter how little content or short, conduct retrospectives!)

## 📞 Support and Feedback

### 💬 Questions and Consultations
- **GitHub Issues**: Bug reports and feature requests
- **Discussions**: Usage questions and consultations
- **Pull Requests**: Improvement proposals and additional features

### 🔄 Continuous Improvement
- **We welcome your feedback**
- **Improvement proposals and additional content are welcome**
- **Share usage examples in the community**

---

**🎉 Let's start collaborative work between AI agents and humans using this package!**

**💡 Don't forget: No matter how little content or short, always conduct retrospectives!**
