# ⚡ FieldForge — Salesforce Schema Deployment Tool

> Deploy custom fields and objects to Salesforce in minutes — no XML, no Setup clicks, no manual metadata editing.

---

## 🚀 One-Click Install

**Sandbox / Developer Org:**

[![Install FieldForge]
https://login.salesforce.com/packaging/installPackage.apexp?p0=04tg50000004farAAA
```

> ⚠️ After installing, complete the post-install setup steps before using the tool.  
> See the **[Installation Guide PDF](./FieldForge_Installation_Guide.pdf)** in this repo for full setup instructions.

---

## 📌 What is FieldForge?

FieldForge is a **Salesforce Lightning Web Component (LWC)** tool that lets Salesforce admins and developers deploy custom fields and objects directly from a CSV or via AI — without touching Setup, Object Manager, or writing a single line of XML.

### The problem it solves

Setting up a data model in Salesforce the traditional way means:
- Clicking through Setup → Object Manager → New Field → 10 screens per field
- No bulk operation — 20 fields = 20 separate workflows
- Easy to make mistakes, hard to undo

FieldForge eliminates all of that.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🤖 **AI Schema Generator** | Describe your app in plain English — FieldForge generates the full CSV schema automatically using Groq AI (Llama 3.3 70B) |
| 📋 **CSV Deployment** | Paste or upload a CSV → preview → deploy. Supports all 23 Salesforce field types |
| 🏗️ **Schema Mode** | Create entire data models from scratch — objects + fields in one operation, in the correct dependency order |
| ➕ **Field Mode** | Add fields to existing objects in bulk |
| ✅ **Preflight Validation** | Checks your org for conflicts (already-existing fields, object limits, relationship errors) before you click Deploy |
| 📊 **Visual Preview** | Grouped view, Flat view, and ERD view before deploying |
| ✏️ **Inline Edit & Delete** | Fix errors directly in the preview table — no need to re-upload CSV |
| ↩ **Undo Deployment** | Deletes everything that was just deployed in one click |

---

## 🎬 How It Works

### AI Mode
1. Open FieldForge on any Lightning page
2. Click **AI Schema Generator**
3. Type: *"Build a hospital management system with patients, doctors and appointments"*
4. Review the generated schema in preview
5. Click **Deploy** — done

### CSV Mode
1. Prepare a CSV with your field definitions
2. Paste it into FieldForge
3. Preflight checks run automatically against your org
4. Fix any highlighted errors inline
5. Click **Deploy**

---

## 📦 Package Details

| | |
|---|---|
| **Package Name** | FieldForge |
| **Version** | 0.1 |
| **Type** | Unlocked Package |
| **Namespace** | None |
| **API Version** | 66.0 |
| **Publisher** | Kunal Kanade |
| **Subscriber Package Version ID** | `04tg50000004farAAA` |

---

## 📋 Post-Install Setup

The tool requires a few one-time configuration steps after installation:

1. Assign the **FieldForge User** permission set to your user
2. Create a **Connected App** in Setup (for Metadata API OAuth)
3. Create an **Auth Provider** linked to the Connected App
4. Configure the **FieldForge_Metadata** Named Credential with OAuth
5. Add your **Groq API Key** in Custom Settings
6. Add the **fieldForge** LWC component to a Lightning page

> 📄 Full step-by-step instructions with screenshots guidance are in the **[Installation Guide PDF](./FieldForge_Installation_Guide.pdf)**

---

## 🛠️ Built With

- **Salesforce LWC** — Frontend UI
- **Apex** — Backend logic, validation, deployment orchestration
- **Metadata API (SOAP)** — Field and object creation/deletion
- **Groq API** (Llama 3.3 70B) — AI schema generation
- **Salesforce Unlocked Package** — Distribution

---

## 👤 Author

**Kunal Kanade**  
Salesforce Developer  






