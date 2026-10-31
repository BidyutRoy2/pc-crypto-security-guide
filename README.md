# 🛡️ Complete PC & Crypto Security Hardening Guide

<img width="1024" height="572" alt="image" src="https://github.com/user-attachments/assets/bfbb6662-e2d5-4be2-b82e-20e3f86282c1" />

> A step-by-step defense guide against infostealers, remote access trojans (RAT), and unauthorized outgoing wallet connections for crypto traders and airdrop hunters. Available in both **Bangla** and **English**.

---

## 📑 Table of Contents / সূচিপত্র
1. [বাংলা সংস্করণ (Bangla Version)](#-বাংলা-সংস্করণ-bangla-version)
   - [Safing Portmaster সেটআপ](#১-safing-portmaster-সেটআপ-ও-ব্যবহার-নির্দেশিকা)
   - [Malwarebytes সেটআপ](#২-malwarebytes-সেটআপ-ও-ব্যবহার-নির্দেশিকা)
   - [Kaspersky Virus Removal Tool (KVRT) সেটআপ](#৩-kaspersky-virus-removal-tool-kvrt-সেটআপ-ও-ব্যবহার-নির্দেশিকা)
2. [English Version](#-english-version)
   - [Safing Portmaster Setup](#1-safing-portmaster-setup--usage-guide)
   - [Malwarebytes Setup](#2-malwarebytes-setup--usage-guide)
   - [Kaspersky Virus Removal Tool (KVRT) Setup](#3-kaspersky-virus-removal-tool-kvrt-setup--usage-guide)
3. [License](#-license)

---

## 🇧🇩 বাংলা সংস্করণ (Bangla Version)

### ১. Safing Portmaster সেটআপ ও ব্যবহার নির্দেশিকা
Portmaster হলো একটি ওপেন-সোর্স কার্নেল-লেভেল অ্যাপ্লিকেশন ফায়ারওয়াল, যা পিসির ব্যাকগ্রাউন্ডে চলা প্রতিটি অ্যাপের নেটওয়ার্ক ট্রাফিক মনিটর করে এবং ইনফোস্টিলারের ডেটা পাচার আটকে দেয়।

#### ক) ডাউনলোড ও ইনস্টলেশন
1. অফিসিয়াল সাইট https://www.safing.io থেকে উইন্ডোজ ইনস্টলারটি ডাউনলোড করুন।
2. ফাইলে রাইট-ক্লিক করে **Run as administrator** দিয়ে ওপেন করুন।
3. ইনস্টলেশন শেষ হলে কার্নেল ড্রাইভার কার্যকর করার জন্য **পিসি অবশ্যই একবার রিস্টার্ট দিন**।

#### খ) সিকিউরিটি কনফিগারেশন
1. টাস্কবার থেকে Portmaster ওপেন করে **Settings > DNS**-এ যান। `Secure DNS` সক্রিয় রেখে **Quad9** (`dns.quad9.net`) সিলেক্ট করুন।
2. **Settings > Global Settings**-এ যান:
   - **Default Network Action:** সাধারণ ব্যবহারের জন্য `Allow`, বা সর্বোচ্চ নিরাপত্তার জন্য `Prompt` দিন।
   - **Block P2P / Direct Connections:** সক্রিয় রাখুন যাতে ব্যাকগ্রাউন্ড টানেল ব্লক থাকে।

#### গ) ক্ষতিকর অ্যাপ ব্লক করার নিয়ম
1. বাম পাশের **Monitor** বা **Apps** ট্যাবে যান।
2. কোনো অচেনা স্ক্রিপ্ট বা ব্যাকগ্রাউন্ড কানেকশন দেখতে পেলে অ্যাপে ক্লিক করে **Block All Connections** টগল অন করে দিন।

---

### ২. Malwarebytes সেটআপ ও ব্যবহার নির্দেশিকা
ইনফোস্টিলার ট্রোজান (Lumma, Stealc) এবং ব্রাউজার হাইজ্যাকার ক্লিন করার জন্য এটি কার্যকর।

#### ক) ইনস্টলেশন ও অন-ডিমান্ড স্ক্যান
1. https://www.malwarebytes.com থেকে ফ্রি ইনস্টলার নামিয়ে রান করুন।
2. ড্যাশবোর্ডের **Scanner** থেকে **Scan** বাটনে ক্লিক করুন।
3. স্ক্যান চলাকালীন ব্রাউজার বন্ধ রাখুন। কোনো ক্ষতিকর ফাইল পাওয়া গেলে **Quarantine** করুন।

#### খ) ১৪ দিন পর ফ্রি মোড ব্যবহার
1. ট্রায়াল শেষে ওপরের **Settings (Gear Icon) > Account** ট্যাবে যান।
2. **Deactivate Premium Trial** বা **Switch to Free** সিলেক্ট করুন। এটি আজীবন ফ্রি অন-ডিমান্ড স্ক্যানার হিসেবে কাজ করবে।

---

### ৩. Kaspersky Virus Removal Tool (KVRT) সেটআপ ও ব্যবহার নির্দেশিকা
এটি একটি পোর্টেবল স্ক্যানার, যা ইনস্টলেশন ছাড়াই মেমোরি ও রুটকিট স্ক্যান করে।

#### ক) কনফিগারেশন ও ডিপ স্ক্যান
1. ক্যাসপারস্কির অফিশিয়াল পোর্টাল থেকে `KVRT.exe` https://www.kaspersky.co.in/downloads/free-virus-removal-tool ডাউনলোড করুন।
2. রাইট-ক্লিক করে **Run as administrator** দিয়ে ওপেন করে লাইসেন্স গ্রহণ করুন।
3. **Change parameters**-এ গিয়ে **System memory**, **Startup objects**, **Boot sectors**, এবং **System drive (C:)** সিলেক্ট করে **OK** দিন।
4. **Start scan**-এ ক্লিক করুন। স্ক্যান শেষে থ্রেট পাওয়া গেলে **Disinfect** বা **Delete** করে পিসি রিস্টার্ট দিন।

---

## English Version

### 1. Safing Portmaster Setup & Usage Guide
Portmaster is an open-source, kernel-level application firewall that inspects inbound and outbound network traffic.

#### A. Installation & Configuration
1. Download from https://www.safing.io and run the installer as administrator.
2. Restart your computer after installation to initialize the kernel network driver.
3. In **Settings > DNS**, enable Secure DNS with Quad9 (`dns.quad9.net`).
4. In **Settings > Global Settings**, enable **Block P2P / Direct Connections**.

#### B. Traffic Inspection & App Blocking
1. Open the **Apps** or **Monitor** view to observe real-time outbound sessions.
2. Click on any suspicious process and activate **Block All Connections**.

---

### 2. Malwarebytes Setup & Usage Guide
Designed to detect zero-day infostealers (Stealc, Lumma) and unauthorized browser modifications.

#### A. Installation & Manual Scanning
1. Download from https://www.malwarebytes.com and complete the personal setup.
2. Open the **Scanner** tab and execute a full scan with browsers closed.
3. Review and quarantine identified malicious binaries.

#### B. Lifetime Free On-Demand Setup
1. After the 14-day trial, navigate to **Settings > Account**.
2. Select **Deactivate Premium Trial** to retain permanent on-demand scanning functionality.

---

### 3. Kaspersky Virus Removal Tool (KVRT) Setup & Usage Guide
A standalone, portable malware cleaner that disinfects hidden memory objects and kernel rootkits.

#### A. Execution & Full Deep Scan
1. Download the latest KVRT.exe https://www.kaspersky.co.in/downloads/free-virus-removal-tool from the official Kaspersky portal.
2. Run as administrator and accept the licensing terms.
3. Click **Change parameters**, select **System memory**, **Startup objects**, **Boot sectors**, and **System drive (C:)**.
4. Click **Start scan**, then disinfect or remove flagged threats upon completion.

---

## 📜 License
Distributed under the MIT License.
