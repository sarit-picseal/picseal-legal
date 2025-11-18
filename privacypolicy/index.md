---
title: PicSeal Privacy Policy
---

# Privacy Policy

**Last updated:** November 18th, 2025

This Privacy Policy describes how **PicSeal** (“**we**”, “**us**”, “**our**”) collects, uses, and shares information when you use our iOS application PicSeal (the “**App**”) and our legal website at `legal.picsealapp.com` (together, the “**Service**”).

If you do not agree with this Policy, please do not use PicSeal.

---

## 1. Who we are & how to contact us

PicSeal is operated by **Quokka LLC**, a company organized in **Minnesota, United States of America**.

- **Email:** contact@picsealapp.com  
- **Address:** [ADDRESS]

We are the “data controller” for personal data we collect through the Service (or the equivalent under your local law).

---

## 2. What we collect

We only collect information we need to operate and improve PicSeal:

1. Information you provide directly  
2. Photos and media you submit  
3. Usage and analytics data  
4. Device and diagnostic data  
5. Information from Apple and other platforms

### 2.1 Information you provide directly

- **Email address**  
  - When you choose to **Sign in with Apple**, we receive either your real email address or an anonymized Apple relay email.  
- **Support communications**  
  - If you contact us, we receive whatever contact details and message content you send.

We do **not** collect passwords. Authentication is handled by Apple and/or our backend provider.

### 2.2 Photos and media you submit

PicSeal has two main parts: **Scan** and **Enhance**. They behave differently for privacy.

#### a) Scanner photos used for ML training (opt-in only)

If you choose to **help improve PicSeal** in the App, we will upload photos captured with the in-app **scanner** for research and development.

- **What we collect**
  - The full image captured through the PicSeal scanner.
- **What we do not collect**
  - Photos you only **import from your photo library** are *not* uploaded for training in the current version.
- **Where they go**
  - Stored temporarily in **Supabase** object storage (on infrastructure such as Amazon S3).  
  - Then transferred to **Roboflow**, a third-party service we use for dataset management, annotation, and model training.
- **How we use them**
  - To train and evaluate computer-vision models that detect and crop individual photos inside a scan.  
  - To understand what people are trying to preserve (for example, prints, albums, and keepsakes) and to design better algorithms or steps in our scanning pipeline.

Once images are transferred to Roboflow, they are stored there as part of our training dataset and **are not linked back to individual users**.

#### b) Photos submitted for enhancement (Replicate AI workflow)

When you use **Enhance** features:

- **What we collect**
  - The photo you select for enhancement.
- **Where they go**
  - Uploaded to Supabase object storage.  
  - Our backend sends a copy to **Replicate** (a third-party AI provider) to run the enhancement model.
- **Retention**
  - Replicate deletes prediction inputs and outputs after about **one hour** by default.  
  - Our copy in Supabase is kept for up to **7 days** for processing, troubleshooting, and quality assurance, and then deleted.
- **How we use them**
  - To deliver the enhancement you requested and to debug failures.  
  - We **do not** use enhancement photos for ML training at this time.

You remain responsible for backing up your original photos elsewhere. PicSeal is not a long-term backup service.

### 2.3 Usage and analytics data

We use privacy-friendly analytics to understand how the app is used and to improve it.

Examples of data:

- App opens and closes  
- Scanner opened / closed  
- Number of photos detected in a scan (for example, “4 photos detected”)  
- Whether auto-crop succeeded or failed  
- Whether enhancement started and completed successfully  
- Whether the “Help improve PicSeal” setting is enabled  
- Device model (e.g., iPhone 15), iOS version, app version, general region

We **do not** collect screen recordings or session replays, and we do **not** send raw images, bounding boxes, or face crops to analytics.

Analytics are currently powered by **PostHog**, which acts as our data processor.

### 2.4 Device and diagnostic data

Apple and our backend may provide:

- Crash reports  
- Performance metrics  
- Error logs (without image content)

We use this solely to debug and improve stability.

### 2.5 Information from Apple / app stores

If you purchase a subscription or in-app purchase:

- Apple processes your payment.  
- We receive high-level information such as the product purchased and anonymized identifiers needed to manage your subscription.

We do **not** receive your full credit-card number or full billing address from Apple.

---

## 3. How we use your information

We use your information to:

1. **Provide the Service**  
   - Run the app, process scans and enhancements, maintain your account.  
   - Legal basis (where applicable): performance of a contract.

2. **Improve PicSeal and develop new features**  
   - Train and evaluate our scanning models using opt-in scanner photos.  
   - Understand which types of memories users are trying to preserve and design new algorithm steps.  
   - Legal basis: your **consent** (for training data) and our **legitimate interests** in improving the Service.

3. **Analytics and usage insights**  
   - Measure feature usage, flows, and performance; prioritize product work and troubleshoot issues.  
   - Legal basis: legitimate interests.

4. **Communicate with you**  
   - Respond to support requests and notify you about important changes.  
   - Legal basis: performance of a contract; legitimate interests.

5. **Safety, security, and legal compliance**  
   - Detect abuse or misuse and comply with legal obligations.  
   - Legal basis: legal obligations; legitimate interests.

---

## 4. When we share information

We do not sell your personal information.

We share information only with:

### 4.1 Service providers (processors)

We use trusted third parties to help us operate the Service:

- **Supabase** – authentication, database, and file storage.  
- **Roboflow** – dataset management, annotation, and ML model training for scanner images (opt-in only).  
- **Replicate** – AI service that performs photo enhancements.  
- **PostHog** – analytics platform for usage metrics.  
- **Apple / App Store / TestFlight** – distribution, in-app purchases, and crash reporting.

These providers act on our instructions and are bound by contracts to protect your data.

### 4.2 Business transfers

If PicSeal or substantially all of our assets are acquired, or we undergo a merger or reorganization, user data (including training datasets and trained models) may be transferred to the acquiring entity as part of the transaction. The new entity will continue to honor this Policy or provide you with notice of any changes.

### 4.3 Legal requirements

We may disclose information if we believe it is reasonably necessary to:

- Comply with applicable law or legal process  
- Protect the rights, property, or safety of our users, the public, or ourselves  
- Enforce our Terms of Service  

---

## 5. How long we keep your information

- **Scanner training photos (opt-in)**  
  - Kept in Supabase long enough to transfer to Roboflow.  
  - At Roboflow, used in our training datasets for as long as needed to develop and operate our models.  
  - Once included in a dataset or trained model, these images are **not individually removable**, because they are no longer linked to specific users.

- **Enhancement photos**  
  - Replicate: deleted after ~1 hour (per their defaults).  
  - Supabase: retained for up to **7 days** for processing and debugging, then deleted.

- **Account and contact info**  
  - Kept while your account is active or as needed to provide the Service and for a reasonable period afterward for record-keeping and legal obligations.

- **Analytics data**  
  - Retained in aggregated or pseudonymous form for as long as useful for understanding usage and improving the app.

We may keep some information longer if required by law.

---

## 6. Your choices and rights

### 6.1 Training data consent & opt-out

- Participation in scanner training is **optional**.  
- You can toggle this setting in the App under **Settings → Help Improve PicSeal** (name may vary).  
  - When turned **off**, we stop uploading new scanner images for training.  
  - Turning it off does **not** remove images already integrated into training datasets or trained models, because we cannot reliably link those images back to your account.

### 6.2 Access, correction, deletion

Depending on your location, you may have legal rights to:

- Request access to personal information we hold about you  
- Request correction of inaccurate information  
- Request deletion of certain information  

You can contact us at **contact@picsealapp.com** to make these requests. We may need to verify your identity.

We will honor valid requests where required by law, subject to limitations—for example, we generally cannot delete:

- Information we are legally required to keep  
- Information already aggregated or anonymized  
- Scanner images already integrated into training datasets or models

---

## 7. International data transfers

Our service providers may process your information in countries other than where you live. Where required, we apply appropriate safeguards (such as standard contractual clauses) to protect your data.

---

## 8. Children’s privacy

PicSeal is **not directed to children under 18**, and we do not knowingly allow children to create accounts.

However, the photos you scan may depict children (e.g., family photos). By using the Service, you confirm that you are an adult and have the right to scan and upload those photos.

If you believe a child has provided us with personal information directly, please contact us and we will take appropriate steps.

---

## 9. Security

We use reasonable technical and organizational measures to protect your information, including encryption in transit, restricted access to production systems, and the use of reputable infrastructure providers.

No system can be 100% secure; we cannot guarantee absolute security.

---

## 10. Changes to this Policy

We may update this Policy from time to time. We will update the “Last updated” date above and, where appropriate, notify you in-app or by other means.

Your continued use of PicSeal after changes become effective means you accept the updated Policy.

---

## 11. Contact

If you have any questions or concerns about this Policy or our data practices, please contact us:

- **Email:** contact@picsealapp.com 
- **Address:** [ADDRESS]
