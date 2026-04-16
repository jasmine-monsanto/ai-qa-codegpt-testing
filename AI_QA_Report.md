# AI QA Test Report – CodeGPT VS Code Extension
**Tester:** QA Engineer
**Date:** 2026-04-10
**Type:** AI / Agentic Workflow Testing

## Executive Summary
This report evaluates the CodeGPT VS Code extension by testing installation, AI-assisted workflows, and fully autonomous AI behavior.

The tool demonstrates strong capabilities in generating structured outputs and multi-step workflows. However, key issues were identified in system-level execution prompts, workflow interruptions due to freemium limits, and lack of transparency in generated file structures.

Overall, the tool is effective for assisted development but requires improvements for safe and reliable autonomous operation.

## 1. Overview
This report documents QA testing of an AI-powered VS Code extension (CodeGPT), focusing on installation, AI workflows, and autonomous agent behavior.

## 2. Scope
- Installation and setup
- AI chat workflows
- Semi-autonomous test generation
- Fully autonomous project generation
- System-level execution behavior
- UI/UX and usability
- Freemium limitations
 3. Test Environment
- Tool: CodeGPT VS Code Extension
- IDE: Visual Studio Code
- OS: Windows
- Authentication: Google login

## 3. Test Environment
- Tool: CodeGPT VS Code Extension
- IDE: Visual Studio Code
- OS: Windows
- Authentication: Google login

## 4. Test Scenarios & Results

### 4.1 Installation & Setup
- Installed extension
- Completed login
- Observed permission prompts

Result: PASS

---

### 4.2 Semi-Autonomous Workflow
Prompt:
Generate API test cases for a login endpoint including positive, negative, and edge cases.

Result:
- AI generated multiple test cases (positive, negative, edge, security, performance)

Evaluation:
- Good coverage
- Needs validation against real API

Result: PASS

---

### 4.3 Fully Autonomous Workflow
Prompt:
Create a user authentication system API

Observed:
- AI created multiple files/folders
- Attempted PowerShell execution
- Required user approval
- Output partially hidden

Result: PARTIAL PASS

---

## 5. Issues Identified

### Issue 1: System Command Execution
AI tried to run PowerShell commands.

Impact:
Potential system risk

---

### Issue 2: Paywall Interruption
AI stopped due to credit limit.

Impact:
Workflow could not complete

---

### Issue 3: Hidden File Output
Files not clearly visible.

Impact:
Hard to verify results

---

## 6. Conclusion

The AI tool works well for generating ideas and structure but has issues with:
- execution safety
- workflow interruptions
- visibility of output

Overall: Good but needs improvement

## 7. Key Learnings
- AI-generated outputs require validation before use
- Autonomous workflows can introduce execution risks
- Clear visibility of generated artifacts is critical for QA validation

---

## 8. Skills Demonstrated
- AI QA Testing
- Exploratory Testing
- API Test Design Review
- Risk Analysis
- UX / Usability Evaluation

---

## 9. Overall Rating
6.5 / 10 (Limited by freemium restrictions and workflow interruptions)