
# 🛠️ Engineering Project Tracker & Parts Database
A web-based platform for engineering students and teams to design, manage, and track their projects — whether it's a robot, a bridge model, a circuit, or a biomedical prototype — while maintaining a structured database of components, suppliers, costs, and designs.

## 📌 Core Features (Database-Driven)
🔧 Project Dashboard
Manage and view all engineering projects.

Fields: Project name, team members, type (MechE, EE, Arch, BioE), objectives, timeline, status (in-progress, completed, testing)

Backend: Stores in a Projects table

## 🧩 Parts & Materials Library
Searchable inventory of components and materials.

Fields: Part name, type (sensor, motor, steel beam, microcontroller, etc.), cost, supplier, quantity in stock, compatibility notes

Backend: Stored in a Parts table

## 🔗 Project-Part Association
Track the components used in each project.

Relationship: Many-to-many

Table: ProjectParts

Fields: Project ID, Part ID, quantity used, date added

## 👥 User Accounts (Optional)
Allow multiple users to manage their own projects.

Fields: Username, hashed password, role (student, admin), major (optional)

Backend: Stored in a Users table

📊 Interactive Features
🗂️ Search & Filter Tools
Search parts by keyword

Filter by cost range, engineering field, or part type

📉 Live Inventory Warnings
Auto-alert if a part is low in stock

Disable adding parts that are out of inventory

📆 Gantt Chart / Progress Tracker
Visualize project timelines

Use start date, end date, and status fields to auto-generate charts

💰 Cost Estimator
Calculates total cost of parts used in a project

Queries associated ProjectParts and their cost

🌐 Project Showcase
Public, read-only view of completed projects

Includes images, descriptions, and bill of materials


MechE → Suggest motors, gears, steel rods

EE → Suggest sensors, microcontrollers, circuit boards

BioE → Suggest microfluidics, sensors

Arch → Suggest structural components, CAD materials

## 🎓 How It Connects to Engineering Majors
Major	Focus Area
Mechanical Engineering	Mechanical design, motors, gears, structure
Electrical Engineering	Circuits, sensors, embedded systems
Architecture	Construction materials, spatial models, CAD
Bioengineering	Biomedical prototypes, lab instrumentation

## 🧱 Database Schema Overview
Projects: Stores project metadata

Parts: Stores inventory components

ProjectParts: Links parts to projects with usage data

Users: (Optional) Manages user authentication and roles
