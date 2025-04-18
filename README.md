## NAME:VIVEK SANJAY PAWAR


# 📚 SAP ABAP CRUD ALV Report for Student Management

## 📖 Project Overview

This project is a **SAP ABAP report** that implements **CRUD operations (Create, Read, Update, Delete)** on a custom **student management table (`ZSTUDENT_DATA`)**, and displays the data using an **ALV (ABAP List Viewer) Grid Report**.

It provides an easy-to-use selection screen where users can input student details and select the desired operation (Insert, Update, Modify, Delete, Display).

---

## 🛠️ Technologies Used

- **SAP ABAP**
- **ALV Grid Display (REUSE_ALV_GRID_DISPLAY)**
- **ABAP Dictionary Tables (`ZSTUDENT_DATA`)**
- **Selection Screen Parameters**
- **ABAP Work Areas & Internal Tables**

---

## 📋 Features

✅ **Insert** new student records  
✅ **Update** existing student records  
✅ **Modify** records in bulk  
✅ **Delete** records by PRN number  
✅ **Display** all student records in an **ALV report**

---

## 📑 Table Structure — `ZSTUDENT_DATA`

| Field Name | Data Element   | Description           |
|------------|----------------|-----------------------|
| `PRN_NO`    | `ZPRN_NO`        | PRN Number (Primary Key) |
| `F_NAME`    | `ZFIRST_NAMEE`   | First Name            |
| `M_NAME`    | `ZMIDDLE_NAME`   | Middle Name           |
| `L_NAME`    | `ZLAST_NAMEE`    | Last Name             |

---

## 📂 Project Structure

ZCRUD_ALV_PROJECT (Report) ├── Selection Screen ├── CRUD Operation Logic ├── ALV Field Catalog Setup └── ALV Grid Display using 'REUSE_ALV_GRID_DISPLAY'


---

## 🖥️ How It Works

### 🔹 Selection Screen:
The report provides a selection screen with:
- **Fields to enter PRN number, First, Middle, and Last Name**
- **Radio buttons** to select one of the operations:
  - Insert  
  - Update  
  - Modify  
  - Delete  
  - Display  

### 🔹 CRUD Operations:
- **Insert**: Adds a new student record to the table.
- **Update**: Updates an existing record matching the given PRN.
- **Modify**: Modifies a record based on PRN.
- **Delete**: Deletes a student record by PRN.
- **Display**: Fetches and shows all records in an **ALV Grid Report**.

### 🔹 ALV Report:
The **ALV Grid Display** shows student details in a tabular format with the following columns:
- PRN Number
- First Name
- Middle Name
- Last Name

---

## 📸 Screenshots (optional)
> You can attach SAP GUI or ALV output screenshots here for better visualization.

---

## 📌 Prerequisites

- SAP system access with **ABAP development authorization**
- Custom **Database Table: `ZSTUDENT_DATA`** created in Data Dictionary
- ABAP Workbench (`SE38`, `SE11`)

---

## 📤 How to Run

1. Open transaction **SE38**
2. Create a report named `ZCRUD_ALV_PROJECT`
3. Paste the ABAP code from this repository
4. Activate the report
5. Execute the report (`F8`)
6. Use the selection screen to perform operations

---

## 💡 Future Enhancements

- Add validations for duplicate PRN numbers
- Include additional fields (Date of Birth, Email, Mobile)
- Export ALV report to Excel or PDF
- Add custom ALV layouts and sorting

---

