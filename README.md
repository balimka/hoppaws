# 🐾Hoppaws - Pet Marketplace Platform Development Plan

This document outlines the structured plan for developing a pet marketplace and service platform. The project is split into **Epics** (main themes) and **Steps** (smaller deliverables), helping visualize progress and estimate time.

---

## 📌 EPIC 1: Landing Page & User Experience

### Steps:
- [ ] Design and implement homepage layout (mobile & desktop-first)


---

## 📌 EPIC 2: Marketplace Core Functionality

### Step 1: Pet Listings
- [ ] Create "Buy a Pet" feature
  - [ ] Listing filters: species, breed, price, location, etc.
  - [ ] Pet detail page with images and info
- [ ] Create "Sell a Pet" feature
  - [ ] Pet listing form with validation (age, breed, health info)
  - [ ] Payment integration for premium listings
- [ ] Create "Adoption" feature
  - [ ] Separate category for adoption-only listings
---

## 📌 EPIC 3: Authentication & User Roles

### Step 1: Role-Based Access
- [ ] Guest user
  - Can browse listings
  - Cannot interact with partner services
- [ ] Registered User
  - Can create listings
  - Can browse services and post service requests
  - Can apply for Partner
  - Can create Service price requests
- [ ] Partner
  - Can create/edit services
  - Can respond to requests
  - See analytics of their offers
- [ ] Admin
  - Full management rights - can add/remove listings, can add/remove categories(e.g. dogs, cats ...)
  - Approve partners
  - View analytics and user interactions

### Step 2: Auth Implementation
- [ ] Register / Login system
- [ ] Role assignment on registration
- [ ] Admin panel to approve Partner status
- [ ] Redirect guests when trying to access restricted content(services without login)

---

## 📌 EPIC 4: Admin Dashboard

### Features:
- [ ] Partner request approvals
- [ ] User and listing management
- [ ] Click tracking dashboard
  - [ ] Listings viewed
  - [ ] Services viewed
  - [ ] Contact reveals (email/phone)
- [ ] Insights and statistics per service or user type

---

## 📌 EPIC 5: Partner Dashboard and Partner core functionality

### Step 1: Features:
- [ ] Create/edit service listings
- [ ] Respond to user requests
- [ ] Analytics: views, contact clicks, offer responses


### Step 2: Service Marketplace 
- [ ] Service Categories
- [ ] Service Page Layout
  - [ ] Overview of services
  - [ ] Filter and search partners by service
- [ ] Partner Profiles
  - [ ] Business name, logo, short bio
  - [ ] Services provided
  - [ ] Reviews & ratings
  - [ ] Contact Info (hidden until clicked)

---

## 📌 EPIC 6: Backend Functionality & Templates

### Step 1: Service Request Flow
- [ ] Create templated request forms per service (e.g. for grooming: pet type, haircut style, etc.)
- [ ] Allow users to submit request to selected service category
- [ ] Notify partners with matching services
- [ ] Partner can send offer (price, message)
- [ ] User can accept/reject offers

### Step 2: Contact Security
- [ ] Hide partner contact info until "Reveal"
- [ ] Log each reveal with timestamp and user

### Step 3: Search & Filter Logic
- [ ] Marketplace filters (species, location, price, etc.)
- [ ] Partner filters (service category, distance, rating)

---

## 📌 EPIC 7: Tracking & Analytics

### Steps:
- [ ] Click Tracking System
  - [ ] Listings views
  - [ ] Partner profile views
  - [ ] Contact reveal counts
  - [ ] Save anonymous and registered users' last interactions
- [ ] Admin & Partner analytics panels

---

## 📌 EPIC 8: Become a Partner & Advanced Features

### Steps:
- [ ] Create “Become a Partner” form (gated behind login)
  - [ ] Info about business, services, availability
  - [ ] Form sends application to admin
  - [ ] Send email notification to admin
- [ ] Admin approval process (manual or auto)
- [ ] Partner upgraded account (new dashboard access)
- [ ] Notification to partner after approval

---

## ✅ Future Considerations
- Chat/messaging between users and partners
- Rating & review system for services/users
- Multi-language support

