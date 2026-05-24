# RTU Faculty Evaluation System

A modern web-based Faculty Evaluation System for Rizal Technological University.

## 🚀 Deployment (GitHub Pages)

1. Upload all files in this folder to your GitHub repository root.
2. Go to **Settings → Pages → Source → Deploy from branch → main → / (root)**.
3. Your site will be live at: `https://<your-username>.github.io/<repo-name>/`

## 📁 File Structure

```
/
├── index.html          ← Main application (all-in-one)
├── images/
│   └── rtu-logo.png   ← Place your RTU logo here (transparent PNG)
└── README.md
```

## 🖼️ Adding the RTU Logo

Place your official RTU logo file inside the `images/` folder and name it exactly:

```
images/rtu-logo.png
```

The system will automatically display it in:
- Login page branding panel
- All dashboard headers (Student, Faculty, Admin)
- Receipt page

> If the image file is missing, an SVG fallback logo is shown automatically.

## 🔐 Default Login Credentials

### Student
| Field          | Value                        |
|----------------|------------------------------|
| Student Number | Any format: `2024-XXXXXX`   |
| Password       | `123456789`                  |

> Students should change their password after first login using **Forgot Password**.

### Faculty
| Faculty Name        | Faculty ID | Password     |
|---------------------|------------|--------------|
| Reyes, Adrian M.    | FAC-1001   | faculty123   |
| Santos, Camille D.  | FAC-1002   | faculty123   |
| Navarro, Ethan J.   | FAC-1003   | faculty123   |
| Cruz, Bianca A.     | FAC-1004   | faculty123   |
| Mendoza, Rafael P.  | FAC-1005   | faculty123   |
| Flores, Nicole T.   | FAC-1006   | faculty123   |
| Garcia, Vincent L.  | FAC-1007   | faculty123   |
| Torres, Samantha C. | FAC-1008   | faculty123   |

### Admin
| Field    | Value      |
|----------|------------|
| Username | `admin`    |
| Password | `admin123` |

## 🔒 Security Notes

- Passwords are hashed before storage (never stored in plaintext).
- Student identities are fully anonymous in Faculty and Admin views.
- Role-based access control prevents unauthorized dashboard access.
- All evaluation data is stored in the browser's `localStorage`.

> **Note:** For production use, integrate Firebase or Supabase for persistent cloud storage and server-side authentication.

## ✅ Features

- Multi-role login: Student / Faculty / Admin
- Dynamic login form per role
- Student evaluation with required comments
- Faculty dashboard (anonymous comments only, no scores)
- Admin dashboard with analytics, filters, PDF export, faculty management
- Evaluation receipt with PDF save & print
- Password change / forgot password flow
- Receipt deduplication fix
- RTU branding with logo fallback
- Fully responsive layout

## 🛠️ Tech Stack

- HTML5
- Tailwind CSS (CDN)
- Vanilla JavaScript (TypeScript-style architecture)
- jsPDF + jsPDF-AutoTable (PDF generation)
- Browser localStorage (data persistence)
