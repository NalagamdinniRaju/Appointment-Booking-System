# 🏥 Prenatal Care Appointment Booking System

![Project Banner](https://res.cloudinary.com/dwiq4s5ut/image/upload/v1740589947/Screenshot_784_rdpip1.png)

A comprehensive platform for managing prenatal care appointments with obstetricians and gynecologists, featuring real-time availability checks and appointment management.

## 🚀 Key Features

- **📅 Appointment Booking**  
  Interactive calendar with real-time doctor availability
- **👩⚕️ Doctor Profiles**  
  Detailed specialist profiles with images and working hours
- **🔔 Real-Time Updates**  
  Instant updates using WebSocket (Socket.IO)
- 📱 **Responsive Design**  
  Mobile-friendly interface
- 📝 **Form Validation**  
  Robust validation for appointment details
- 🔄 **CRUD Operations**  
  Full Create, Read, Update, Delete functionality for appointments

## 🛠 Tech Stack

### **Frontend**  
![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=white)
![React Router](https://img.shields.io/badge/-React_Router-CA4245?logo=react-router&logoColor=white)
![Axios](https://img.shields.io/badge/-Axios-5A29E4?logo=axios&logoColor=white)
![Radix UI](https://img.shields.io/badge/-Radix_UI-161618)

### **Backend**  
![Node.js](https://img.shields.io/badge/-Node.js-339933?logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/-Express-000000?logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white)
![Socket.IO](https://img.shields.io/badge/-Socket.IO-010101?logo=socket.io&logoColor=white)

### **Utilities**  
![date-fns](https://img.shields.io/badge/-date_fns-003399)
![React Datepicker](https://img.shields.io/badge/-React_Datepicker-0088CC)

## ⚙️ Installation

1. **Clone Repository**
   ```bash
   git clone https://github.com/yourusername/appointment-booking-system.git
   cd appointment-booking-system
   ```

2. **Backend Setup**
   ```bash
   cd server
   npm install
   cp .env.example .env
   # Update MongoDB URI in .env
   ```

3. **Frontend Setup**
   ```bash
   cd ../client
   npm install
   ```

## 🖥 Running the Application

1. **Start Backend**
   ```bash
   cd server
   npm start
   ```

2. **Start Frontend**
   ```bash
   cd ../client
   npm start
   ```

Access the application at `http://localhost:3000`


## 🌟 Key Components

### `AppointmentBooking.js`
- Interactive date/time picker with live availability checks
- Doctor profile display with working hours
- Multi-step confirmation process with modal

### `AppointmentManagement.js`
- Calendar-style appointment listing
- Drag-and-drop rescheduling (future implementation)
- Real-time updates via WebSocket

### `DoctorList.js`
- Grid layout for specialist display
- Search/filter functionality
- Detailed doctor profiles

## 📝 Database Models

```javascript
// Doctor Model
{
  name: String,
  specialization: String,
  working_hours: {
    start: String,
    end: String
  },
  image_url: String
}

// Appointment Model
{
  doctorId: ObjectId,
  date: Date,
  duration: Number,
  appointmentType: String,
  patientName: String,
  notes: String
}
```

## 🤝 Acknowledgements

Special thanks to:
- [Lucide Icons](https://lucide.dev) for medical-themed icons
- [React Datepicker](https://reactdatepicker.com) for intuitive date selection
- [date-fns](https://date-fns.org) for modern date formatting

---
