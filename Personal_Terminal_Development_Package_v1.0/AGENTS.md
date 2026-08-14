# Personal Terminal — AGENTS.md
Version: 1.0
Baseline: Personal Terminal v1.1

## 1. Purpose
This repository develops Personal Terminal, a PWA-style personal dashboard that integrates schedule, tasks, activities/learning, and AI support.

## 2. Baseline Rule
- Personal Terminal v1.1 is the baseline reference version.
- Do not destroy, overwrite, or remove baseline behavior without an explicit task instruction.
- Prefer incremental changes.
- Work on one clearly defined task at a time.

## 3. Project Owner
The project owner is a non-engineer.
When reporting work:
- avoid unexplained engineering jargon;
- explain changes in plain Japanese;
- distinguish “what changed”, “why”, and “what to check”;
- never hide unresolved issues.

## 4. Development Principles
- HTML / CSS / JavaScript are the default technologies.
- Keep dependencies minimal.
- Do not introduce frameworks or build systems unless the task explicitly requires them.
- Prioritize iPad, iPhone, and mobile usability.
- Keep PWA compatibility in mind.
- Separate UI, data, application logic, and AI integration as much as practical.
- Preserve data compatibility where possible.
- Prefer configuration over duplicated code.

## 5. User Modes
The architecture must be able to support:
- standard
- kids
- junior
- student
- senior

Do not fully implement all modes unless instructed.
Mode-specific UI must reuse common core functions where possible.

## 6. Safety Rules for Editing
Before editing:
1. Read this AGENTS.md.
2. Read `docs/00_PROJECT_OVERVIEW.md`.
3. Read `docs/01_REQUIREMENTS.md`.
4. Read `docs/02_ARCHITECTURE.md`.
5. Read `docs/07_TASKS.md`.
6. Inspect the existing code relevant to the task.

Do not:
- delete working features without explicit approval;
- rewrite the whole application for a small task;
- change unrelated files without a clear reason;
- add network/API dependencies without explicit instruction;
- expose secrets, API keys, or personal data.

## 7. Task Execution Policy
For each task:
1. State the task you understand.
2. Inspect the relevant code.
3. Make the smallest reasonable change.
4. Run available checks/tests.
5. Verify that existing core behavior still works.
6. Update `docs/08_CHANGELOG.md` if the task is completed.
7. Report the result.

## 8. Completion Report Format
After implementation, report in Japanese:

### 実施したこと
- ...

### 変更したファイル
- ...

### 動作確認
- ...

### 既存機能への影響
- ...

### 未解決事項
- ...

### 次の推奨作業
- ...

## 9. Definition of Done
A task is done only when:
- the requested behavior is implemented;
- no obvious console/runtime error was introduced;
- baseline behavior relevant to the task remains usable;
- the completion report is provided;
- any unresolved issue is explicitly stated.
