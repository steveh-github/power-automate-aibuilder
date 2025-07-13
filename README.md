# 🌀 Power Automate Flow: Invoice Extraction from SharePoint

This repository contains an exported Microsoft Power Automate flow that loops through all PDF documents in a **specified SharePoint folder** and extracts structured invoice data using the **AI Builder Prebuilt Invoice Processing model**.

---

## 📦 Contents

- `InvoiceExtractionFlow.zip` – Exported Power Automate solution (ZIP format)
- `README.md` – Documentation for understanding and deploying the flow

---

## 🚀 Use Case

This flow is designed to:

1. Traverse all files within a specific SharePoint folder
2. Identify and process only **PDF** documents
3. Extract invoice metadata using AI Builder (e.g., Invoice ID, Vendor, Total)
4. Log, notify, or store extracted data (e.g., SharePoint list, Excel, email, etc.)

Ideal for businesses or departments that handle **bulk invoice uploads to SharePoint** and need automated data extraction.

---

## 🧠 Power Automate Features Used

- SharePoint connector:
  - `Get files (properties only)`
  - `Get file content`
- Control:
  - `Apply to each`
  - `Condition`
- AI Builder:
  - `Extract information from invoices`
- Optional:
  - `Compose`, `Append to array`, `Send an email`, `Create item` in SharePoint list

---

## 🔧 Requirements

- Power Automate license with **AI Builder credits**
- Access to a SharePoint site and folder containing invoice PDFs
- Power Platform environment for importing the solution
- (Optional) SharePoint list or storage target for extracted data

---

## 🛠️ How to Import the Flow

1. Open [Power Automate](https://make.powerautomate.com/)
2. Navigate to **Solutions** → Click `Import solution`
3. Upload the `InvoiceExtractionFlow.zip`
4. Resolve any connection references (e.g., SharePoint, AI Builder)
5. Save and test the flow

---

## 📌 Notes

- Only PDF files are processed; you can customize MIME/type filtering as needed
- AI Builder will consume credits per page processed
- Extraction accuracy may vary based on invoice layout complexity

---

## 📄 License

This project is released under the MIT License. See [LICENSE](LICENSE) for more information.

---

## ✍️ Author

Built and exported using **Power Automate Desktop & Cloud**, and version-controlled with **GitHub Desktop**.

---

## 📬 Feedback / Contributions

Feel free to open issues or submit PRs for enhancements like:
- CSV export
- Email notification on failed AI parse
- Support for multiple invoice formats

---

