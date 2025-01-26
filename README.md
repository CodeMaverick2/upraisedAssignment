
# 🕵️ IMF Gadget Management API  

A top-secret API for managing the Impossible Mission Force's most advanced gadgets. Handle with extreme caution!  

## 🚀 Features  

- 🎭 Randomly generated codenames for each gadget  
- 💥 Self-destruct sequences with confirmation codes  
- 📊 Mission success probability calculations  
- 🔐 JWT Authentication  
- 📡 Real-time status monitoring  

## 🛠️ Quick Start  

```bash  
# Clone this classified repository  
git clone https://github.com/CodeMaverick2/upraisedAssignment.git

# Install dependencies (careful with those packages!)  
npm install   

# Launch the mission  
npm run dev  
```  

## 🎯 API Endpoints  

### Get JWT Token  

```http  
POST /api/test-token  
```  

### Gadget Operations  

```http  
GET    /api/gadgets          # Retrieve all gadgets (Clearance Level 3 required)  
POST   /api/gadgets          # Add a new gadget to the arsenal  
PATCH  /api/gadgets/:id      # Modify gadget specifications  
DELETE /api/gadgets/:id      # Decommission gadget (automatically triggers cover story)  
```  

### Special Operations  

```http  
POST /api/gadgets/:id/self-destruct  
```  
⚠️ **WARNING**: This endpoint will trigger an actual self-destruct sequence. Use with extreme caution!  

## 🎮 Testing with Postman  

1. Get your JWT:  

   ```http  
   POST http://localhost:3000/api/test-token  
   ```  

2. Add to all requests:  

   **Headers:**  
   ```
   Authorization: Bearer your-secret-token  
   ```  

3. Create a gadget:  

   ```json  
   POST /api/gadgets  
   {  
     "name": "Exploding Bubblegum",  
     "description": "Looks like gum, acts like C4"  
   }  
   ```  

## 🔧 Sample Gadget Response  

```json  
{  
  "codename": "The Shadow Hawk",  
  "name": "Exploding Bubblegum",  
  "description": "Looks like gum, acts like C4",  
  "status": "Active",  
  "missionSuccessProbability": 85,  
  "_id": "classified"  
}  
```  

## 🚨 Security Notice  

This API is protected by:  
- JWT Authentication  
- IMF's quantum encryption  
- Self-destructing database entries  
- Multiple failsafe protocols  

## 🎬 Mission Status Codes  

- **200**: Mission Accomplished  
- **201**: Asset Created  
- **401**: Disavowed  
- **403**: Security Breach Detected  
- **404**: Agent/Asset Missing  
- **500**: Mission Critical Failure  

## ⚠️ Warning  

This README will self-destruct in 5 seconds... 🔥  

---

## 📝 License  

**Top Secret** - IMF Classified - Level 7 Clearance Required  

--- 