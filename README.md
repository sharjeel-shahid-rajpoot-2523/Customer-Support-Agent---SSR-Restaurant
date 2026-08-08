_____________________________________________________________________________________________________________________________________________________________________________

🍽️ SSR Restaurant – WhatsApp AI Customer Support & Ordering Automation
_____________________________________________________________________________________________________________________________________________________________________________
An AI-powered WhatsApp customer support and ordering automation system built for **SSR Restaurant** using **n8n, Groq, WAHA, and Google Sheets**.
The system works as an automated restaurant assistant that communicates with customers, provides menu information, answers FAQs, manages conversations, collects orders, and stores confirmed orders in Google Sheets.

_____________________________________________________________________________________________________________________________________________________________________________

🚀 Features
_____________________________________________________________________________________________________________________________________________________________________________
🤖 AI Customer Support:
- Automated WhatsApp customer conversations
- Natural and conversational responses
- Supports English and Urdu
- Professional restaurant customer service
- Handles greetings and customer requests

🍔 Interactive Menu:
- Retrieves menu information from Google Sheets
- Displays menu categories and food items
- Provides:
  - Item names
  - Prices
  - Descriptions
  - Sizes
  - Variants
  - Add-ons

🛒 Automated Ordering:
Customers can:
- Add multiple food items
- Change quantities
- Select sizes and variants
- Add or remove add-ons
- Modify their order before confirmation
- Review the complete order summary

✅ Order Confirmation:
Before placing an order, the AI provides:
- Ordered items
- Quantities
- Variants/sizes
- Add-ons
- Subtotal
- Delivery charges
- Final payable amount

The customer must explicitly confirm the order before it is placed.

👤 Customer Information:
After confirmation, the system collects:
- Full Name
- Phone Number
- Delivery or Dine-in
- Payment Method
- Delivery Address when required

💳 Payment Handling:
Supports:
- Online Payment
- Cash on Delivery

Online payment instructions can be provided through the automated assistant.

📊 Google Sheets Integration:

Google Sheets is used as the restaurant's information and order-management database.

The workflow includes:

- 🍔 Menu
- 🏪 Restaurant Information
- ❓ FAQs
- 📦 Orders

🧠 Conversation Memory:
The AI agent uses conversation memory to maintain context during customer conversations.
The customer's WhatsApp number is used as the conversation session key.

📱 WhatsApp Automation:
The system:
1. Receives WhatsApp messages
2. Sends them to n8n
3. Processes them through the AI Agent
4. Retrieves information from Google Sheets when required
5. Generates an AI response
6. Sends the response back to WhatsApp

_____________________________________________________________________________________________________________________________________________________________________________

📸 Screenshots
_____________________________________________________________________________________________________________________________________________________________________________

🔄 n8n Automation Workflow: 

![n8n Workflow](<Customer Support Agent - SSR Restaurant - Workflow.jpeg>)

💬 WhatsApp AI Customer Support

![WhatsApp Customer Support](<Customer Support Agent - SSR Restaurant (1).jpeg>)

🍔 Menu & Customer Interaction

![Menu Interaction](<Customer Support Agent - SSR Restaurant (2).jpeg>)

🛒 Automated Ordering

![Automated Ordering](<Customer Support Agent - SSR Restaurant (3).jpeg>)

✅ Order Confirmation

![Order Confirmation](<Customer Support Agent - SSR Restaurant (4).jpeg>)

📦 Customer Support Flow

![Customer Support Flow](<Customer Support Agent - SSR Restaurant (5).jpeg>)

📊 Order / Data Management

![Data Management](<Customer Support Agent - SSR Restaurant (6).jpeg>)

_____________________________________________________________________________________________________________________________________________________________________________

🎥 Project Demo
_____________________________________________________________________________________________________________________________________________________________________________

Watch the complete SSR Restaurant WhatsApp AI Customer Support automation in action.

▶️ **[Watch Project Demo](https://youtu.be/eRCEcAYeKJI?si=UCLte3eFf1UVJe8q)**

_____________________________________________________________________________________________________________________________________________________________________________

🏗️ Workflow Architecture
_____________________________________________________________________________________________________________________________________________________________________________
```text
                👤 Customer
                     │
                     ▼
               📱 WhatsApp
                     │
                     ▼
                  🔗 WAHA
                     │
                     ▼
               🌐 n8n Webhook
                     │
                     ▼
                🤖 AI Agent
                     │
          ┌──────────┼───────────┐
          │          │           │
          ▼          ▼           ▼
       🧠 Memory   🧠 Groq    📊 Google Sheets
                                  │
                    ┌─────────────┼─────────────┐
                    │             │             │
                    ▼             ▼             ▼
                  Menu      Restaurant Info    FAQs
                                  │
                                  ▼
                                Orders
                     │
                     ▼
               🤖 AI Response
                     │
                     ▼
                  🔗 WAHA
                     │
                     ▼
               📱 WhatsApp
                     │
                     ▼
                👤 Customer
