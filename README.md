# 💳 Bill Payment Reminder Bot - UiPath

This UiPath RPA project is designed to automate bill payment reminders via email. It reads customer bill details from an Excel file and sends personalized email reminders, tracks email statuses, handles exceptions, and updates the Excel file accordingly.

## 📌 Features

- ✅ Reads customer details including:
  - Customer Name
  - Bill Name
  - Due Date
  - Amount
  - Email Address
- 📧 Sends personalized email reminders automatically
- 🔔 Notifies user if any email fails to send
- 📊 Generates a summary of email status
- 📂 Easy to customize and extend

---

## 📁 Project Structure



BillPaymentReminderBot/
├── Data/
│   └── BillDetails.xlsx          # Input/Output Excel file
├── Main.xaml                     # Main workflow file
├── Config/
│   └── config.xlsx (optional)    # Stores credentials or constants
├── Screenshots/                  # Optional: For UI references
└── README.md                     # Project documentation


---

## ⚙️ Prerequisites

- UiPath Studio (2021.10 or higher recommended)
- SMTP/Outlook configured for sending emails
- Excel file (`BillDetails.xlsx`) in the following format:

| CustomerName | Email            | BillName     | DueDate   | Amount | EmailStatus |
|--------------|------------------|--------------|-----------|--------|-------------|
| John Doe     | john@example.com | Electricity  | 10-Jun-25 | 1200   |             |

---

## 🚀 How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/BillPaymentReminderBot.git

2. **Open in UiPath Studio**

   * Open `Main.xaml` using UiPath Studio.

3. **Configure Email**

   * Update SMTP/Outlook settings in the workflow or use `config.xlsx`.

4. **Run the Bot**

   * Click **Run** to start the bot.
   * The bot reads from `BillData.xlsx`, sends email reminders, and updates the status.

5. **Review Results**

   * Open the Excel file to check which emails were sent and which failed.

---

## 🛠 Technologies Used

* UiPath Studio
* Excel Application Scope
* SMTP/Outlook Email Activities
* DataTable Manipulation

---

## 📷 Screenshots (Optional)
I can implement my project in two method of criteria there are:

First Method of Implement (Main(Autosaved)):
This method is simple and easy to implement, methodologies of activity is (Input Dialog,Message Box,Assign,Email connection(SMTP),Log Message (or) Write Line)
![Screenshot 2025-06-08 211233](https://github.com/user-attachments/assets/06c3c5bb-25c3-457d-b797-e786872df565)


Second Method of Implement (Main(Fixed)):
This method is similar but literaly simple to implement, methodologies of activity is (Excel Application scope,Input Dialog,Assign,Email connection(SMTP),Log Message (or) Write Line)
![Screenshot 2025-06-08 211205](https://github.com/user-attachments/assets/01dd9d34-ea4d-4fbc-83e9-6c076d708230)


Use any one of the method to implement the project

---

## 💡 Future Enhancements

* Add email template customization
* Dashboard for status reporting
* Schedule bot with UiPath Orchestrator
* Integrate with Google Sheets or databases

```

---

Let me know if you'd like the actual `README.md` file as a downloadable text or markdown file.
```
