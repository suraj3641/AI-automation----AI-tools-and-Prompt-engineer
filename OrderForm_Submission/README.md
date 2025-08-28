# Order Form  submission

# 👕 Super Cool LED T-Shirt Pre-order Automation  
This project automates the **pre-order process** for the "Super Cool LED T-Shirt" using **n8n**.  
It captures customer details via a form, logs them into **Google Sheets**, and sends automated **confirmation & follow-up emails** using Gmail.  


## System Architecture  

# 📝 Pre-order Form  
[T-Shirt Pre-order Form](./Form.png)  

#🔄 Workflow Automation  
[Order Form Submission Workflow](./workflow.png)  

 **Live Pre-order Form**: [Try it here](https://surajmaurya1.app.n8n.cloud/form/3e94e082-39c3-4b85-a5a2-a9f6b19ebb50) 



## 🚀 Introduction  

Instead of manually handling pre-orders, this system fully automates the process:  

- Customers submit their **LED T-Shirt pre-order form** (Name, Email, Phone, Address, Size, Quantity, Color, Payment Method).  
- Data is stored automatically in **Google Sheets**.  
- Conditions are applied (e.g., payment method, size availability).  
- Customers receive **confirmation emails** instantly.  
- Admin also gets notified with order details.  

This ensures a smooth and professional pre-order experience.  


## ✨ Features  

- ✅ **Custom Form** for LED T-Shirt Pre-orders  
- ✅ Auto-store data in Google Sheets for tracking  
- ✅ Condition checks with Filters & Switches  
- ✅ Instant **Email Confirmation** to customers  
- ✅ Multiple paths for different order/payment conditions  
- ✅ Admin Notification Emails  
- ✅ Scalable for any product pre-order system  

---

## 🛠️ Tech Stack  

- **Automation Platform**: n8n  
- **Form Handling**: n8n Form Node  
- **Data Storage**: Google Sheets  
- **Communication**: Gmail (Email Automation)  
- **Workflow Logic**: Filter, Switch, Merge Nodes  

---

## ⚙️ Workflow Explanation  

1. **Customer fills out the Pre-order Form**  
   - Inputs: Name, Email, Phone, Address, Size, Quantity, Color, Payment Method.  

2. **On Form Submission (n8n)**  
   - Triggers workflow automatically.  

3. **Append or Update Row in Sheet (Google Sheets)**  
   - Stores the order details in Google Sheets for tracking.  

4. **Filter Node**  
   - Validates if all required details are filled properly.  

5. **Switch Node**  
   - Routes workflow depending on conditions like **payment method** or **size availability**.  

6. **Send Message (Customer Email)**  
   - Sends confirmation email to the customer with order summary.  

7. **Send Message (Alternative Path)**  
   - Sends an alternate message if payment or stock conditions vary.  

8. **Merge Node**  
   - Combines outputs into one final flow.  

9. **Send Final Notification (Admin Email)**  
   - Admin receives all details for processing and delivery.  

---

## 📊 Example Use Case  

📥 A customer fills out the pre-order form for a **Black LED T-Shirt, Size L, Qty 2, UPI Payment**.  

➡ Workflow automatically:  
1. Stores the order in Google Sheets  
2. Sends customer a **confirmation email** with order details  
3. Notifies the admin with the order info  

---

## 🔧 Tools in n8n  

- **Form Node** → Customer pre-order form  
- **Google Sheets Append/Update** → Store orders  
- **Filter Node** → Validate entries  
- **Switch Node** → Apply conditions (payment/size)  
- **Gmail Send Message** → Customer confirmation emails  
- **Merge Node** → Combine multiple paths  
- **Admin Notification Email** → Keeps admin updated  

