# 🍕 Crustora  
**A Full-Stack Food Ordering Platform with Real-World UX and Scalable Backend Integration**

🔗 Live Demo: https://crustora.netlify.app/

---

## 📌 Overview

Crustora is a production-oriented food ordering web application designed to simulate real-world product behavior.  
It focuses on secure authentication, persistent state management, and frictionless ordering workflows.

The platform enables users to browse items, manage carts, place orders, and seamlessly complete orders via external communication channels.

---

## 🚀 Core Features

### 🔐 Authentication & Session Management
- OTP-based authentication flow  
- Persistent sessions using backend-managed authentication  
- Secure logout with complete session invalidation  
- Automatic session revalidation on reload  

### 🛒 Cart Management
- Dynamic cart operations (add/remove/update items)  
- Persistent cart state across sessions  
- Optimized user flow with minimal friction  

### 📦 Order System
- User-specific order creation and storage  
- Order history tracking  
- Structured data handling via backend services  

### 💬 External Order Workflow
- Seamless redirection to WhatsApp / Instagram for order confirmation  
- Structured order message generation  
- Clipboard fallback for reliability  
- Real-time user feedback via toast notifications  

### 🎯 User Experience Enhancements
- Context-aware toast notifications (success, error, system feedback)  
- Well-defined empty states for better usability  
- Smooth and guided user flow from browsing to order placement  

---

## 🧠 Architecture & Tech Stack

### Frontend
- Next.js / React  
- TypeScript  
- Tailwind CSS  
- ShadCN UI (if applicable)  

### Backend
- Appwrite (Authentication, Database, Session Management)  

### Deployment
- Netlify  

---

## ⚙️ Key Engineering Highlights

- Robust session persistence and validation across reloads and tabs  
- Secure user-scoped data access (orders, profile)  
- Integration of Clipboard API for fallback UX reliability  
- External workflow integration using deep linking (WhatsApp/Instagram)  
- Consistent error handling and feedback mechanisms  

---

## 🔄 Application Flow

1. User browses available items  
2. Adds items to cart  
3. Authenticates via OTP (if not logged in)  
4. Places order  
5. Application:
   - Generates structured order summary  
   - Copies details to clipboard  
   - Redirects user to WhatsApp/Instagram  
6. User confirms order externally  

---

## 🧪 Potential Enhancements

- Payment gateway integration (Stripe / Razorpay)  
- Real-time order tracking system  
- Admin dashboard for order and inventory management  
- Notification system (email/SMS/push)  
- Multi-device cart synchronization  

---

## 🏁 Getting Started

```bash
git clone https://github.com/your-username/crustora.git
cd crustora
npm install
npm run dev
```

---

## 🔐 Environment Configuration

Create a `.env` file in the root directory:

```env
NEXT_PUBLIC_APPWRITE_ENDPOINT=your_endpoint
NEXT_PUBLIC_APPWRITE_PROJECT_ID=your_project_id
```

---

## 📚 Key Learnings

- Designing real-world authentication systems using OTP  
- Managing persistent application state across sessions  
- Building user-centric workflows with fallback mechanisms  
- Integrating frontend applications with Backend-as-a-Service (Appwrite)  
- Handling edge cases and failure scenarios in production-like environments  

---

## 👨‍💻 Author

Neeraj Joshi

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!
