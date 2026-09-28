# Your Doctor (Hackprix)

> A multi-page static website where people with disabilities can find specialist doctors, trainers, partner hospitals and medical training schools, and submit a short consultation form, all from home.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

Built for **Hackprix** (files uploaded in June 2024).

## ✨ Pages

| Page | File | What it shows |
| --- | --- | --- |
| Home | `first pg/yourdoctor.html` | Landing page with navigation, intro ("Consult with our expert doctors and trainers from the comfort of your own home"), featured therapists and trainers, **Get Started** button |
| Get Started | `get started/get started.htm` | Consultation questionnaire (type of disability, duration, cause, age) → Submit (goes to the thank-you page; nothing is sent anywhere) |
| Thank You | `submit/submit.html` | Confirmation after submitting, with a link back home |
| Doctors | `doctors/dotors.html` | Available doctors with specialty, experience and consultation hours |
| Gallery | `gallery/gallery.html` | Therapists with patient success stories, plus partner hospitals |
| Hospitals | `hospitals/hospitals.html` | Hospitals near you and their specialties/facilities |
| Schools | `schools/schools.html` | Medical schools offering training programmes |
| My Profile | `my profile/profil.html` | User menu mock-up (edit name, edit contact number, help & support; the items are placeholders) |

> All doctor, hospital and school entries are **sample/placeholder content** for the prototype.

## 🛠️ Tech Stack

Plain **HTML5 + CSS3**: one stylesheet per page, no JavaScript and no build step.

## 🚀 Running Locally

The site is static and all links are relative, so you can open `wp clone web/first pg/yourdoctor.html` directly in a browser, or serve the folder with any local web server:

```bash
cd "wp clone web"
python -m http.server 5500
# open http://127.0.0.1:5500/first%20pg/yourdoctor.html
```

> Notes: folder names contain spaces (`first pg`, `get started`, `my profile`), and there is no root `index.html`. To publish on GitHub Pages, add an `index.html` that links or redirects to `first pg/yourdoctor.html`. Only the home page has the navigation bar; the other pages don't link back to it.

## 📁 Project Structure

```
wp clone web/
├── first pg/        # home page (yourdoctor.html) + images + style.css
├── get started/     # consultation form
├── submit/          # thank-you page
├── doctors/         # doctors listing
├── gallery/         # success stories + partner hospitals
├── hospitals/       # hospitals listing
├── schools/         # training schools listing
└── my profile/      # user menu
```

## 🗺️ Ideas for next steps

- Add navigation back to the home page on every page
- Make the consultation form actually submit (e.g. Formspree or a small backend)
- Responsive layout review and accessibility pass (alt text, contrast, keyboard navigation). These matter especially for an audience with disabilities

## 📄 License

No licence file has been added yet, so all rights are reserved by default.
