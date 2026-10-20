# ⛪ Church Member Management System

![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
![Excel](https://img.shields.io/badge/Excel-VBA-217346)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-Apps%20Script-34A853)
![GitHub stars](https://img.shields.io/github/stars/mangpijasuan/church-member-management?style=social)

**Free and open source** — created by **[Mangpi Jasuan](https://github.com/mangpijasuan)**.
If it helps your church, please ⭐ **star this repo** and share it!

A church member directory for **Excel** and **Google Sheets**:
member profiles with search, households/families, dashboard, and a data-entry form.

> ⚠️ The workbook in this repo contains **sample data only**. Never commit real member
> names, phones, addresses, or photos. Keep your live copy outside this folder (or in `data/`, which is git-ignored).

## Features
- **Member Profile** – search by name or ID, photo, contact, church and personal details
- **Members** – database with dropdowns, auto Full Name / Age / Birth Month
- **Households** & **Family View** – group members by family (HH-### IDs)
- **Dashboard** – totals, birthdays this month, counts by ministry/group, chart
- **Member Form** – add / edit / delete / search / photos / new household
  - Excel: VBA UserForm (`excel/vba`)
  - Google Sheets: Apps Script dialog (`google-sheets`)

## Folder structure
```
excel/
  Church_Member_Management.xlsx   template workbook (sample data)
  vba/modMemberForm.bas           module: menu macros + button creator
  vba/frmMember.txt               code for the frmMember UserForm
google-sheets/
  Code.gs                         Apps Script server code + menu
  MemberForm.html                 the form UI
```

## Setup – Excel
1. Save the workbook as **.xlsm**.
2. `Alt+F11` → File > Import File → `excel/vba/modMemberForm.bas`.
3. Insert > UserForm → rename it `frmMember` → View Code → paste `frmMember.txt`.
4. Run `CreateFormButtons` once (`Alt+F8`).

## Setup – Google Sheets
1. Upload the .xlsx to Drive → File > Save as Google Sheets.
2. Extensions > Apps Script → paste `Code.gs`; add HTML file `MemberForm` → paste `MemberForm.html`.
3. Reload → **⛪ Church Members > Run Setup (first time only)**.

## Sheet / column rules
The scripts find data by position, so keep the sheet names
(`Members`, `Households`, `Lists`, `Member Profile`, `Family View`) and the Members column order unchanged.

## Download
Go to **[Releases](https://github.com/mangpijasuan/church-member-management/releases)** and download the latest zip.

## Using this template? Tell me! 🙏
Open an issue titled **"We're using it"** with your church name and city (optional) —
it helps me see who it's helping and what to improve. Questions and feature requests are welcome in **Issues**.

## Credit
This project is MIT licensed: you can use, modify, and share it freely, including for your church or organization.
Please keep the copyright notice and the "Created by Mangpi Jasuan" line in any copy you share. Suggested credit:

> Church Member Management template by Mangpi Jasuan — https://github.com/mangpijasuan/church-member-management

## Author
**Mangpi Jasuan** · [GitHub](https://github.com/mangpijasuan) · [Website](https://mangpijasuan.github.io/MJ)
