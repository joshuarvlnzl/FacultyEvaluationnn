# RTU Faculty Evaluation System

A modern web-based Faculty Evaluation System for Rizal Technological University.

## 🚀 Deployment (GitHub Pages)

1. Upload all files in this folder **directly to your GitHub repository root**.
2. Go to **Settings → Pages → Source → Deploy from branch → main → / (root)**.
3. Your site will be live at: `https://<your-username>.github.io/<repo-name>/`

## 📁 File Structure

```
/ (repository root)
├── index.html        ← Main application (all-in-one)
├── rtu-logo.png      ← Place your RTU logo HERE (at root, not in a folder)
├── .nojekyll         ← Prevents GitHub Pages build issues
└── README.md
```

## 🖼️ Adding the RTU Logo

Place your official RTU logo file **directly in the root folder** (same level as index.html) and name it exactly:

```
rtu-logo.png
```

> If the image file is missing, an SVG fallback logo is shown automatically.

## 🔐 Default Login Credentials

The login form auto-detects the account type from the username format — no role selection needed.

### Student
| Field          | Value                       |
|----------------|-----------------------------|
| Username       | Any format: `2024-XXXXXX`  |
| Password       | `123456789`                 |

### Faculty
| Faculty Name        | Username  | Password   |
|---------------------|-----------|------------|
| Reyes, Adrian M.    | FAC-1001  | faculty123 |
| Santos, Camille D.  | FAC-1002  | faculty123 |
| Navarro, Ethan J.   | FAC-1003  | faculty123 |
| Cruz, Bianca A.     | FAC-1004  | faculty123 |
| Mendoza, Rafael P.  | FAC-1005  | faculty123 |
| Flores, Nicole T.   | FAC-1006  | faculty123 |
| Garcia, Vincent L.  | FAC-1007  | faculty123 |
| Torres, Samantha C. | FAC-1008  | faculty123 |

### Admin
| Username | Password  |
|----------|-----------|
| admin    | admin123  |

## ✅ Features
- Auto-detect login role from username (no role tabs)
- Student evaluation with required comments
- Faculty dashboard: anonymous comments only, no scores
- Admin dashboard: analytics, filters, PDF export, faculty management
- Evaluation receipt with PDF save & print
- Password change / forgot password flow
- Receipt deduplication fix
- RTU branding with logo fallback
