# Your Doctor (Hackprix)

> A multi-page static website where people with disabilities can find specialist doctors, trainers, partner hospitals and medical training schools, and submit a short consultation form, all from home.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

Built for **Hackprix** (June 2024). [TODO: confirm event name/format, team members and your role]

Once GitHub Pages is enabled, the site will live at `https://syedbilal04.github.io/Hackprix/`.

## ✨ Pages

| Page | File | What it shows |
| --- | --- | --- |
| Home | `first pg/yourdoctor.html` | Landing page with navigation, intro ("Consult with our expert doctors and trainers from the comfort of your own home"), featured doctors and trainers, partner hospitals, and a **Get Started** button |
| Get Started | `get started/get started.htm` | Consultation questionnaire (page heading: "Consolation Page"; disability, duration, cause, age) → Submit |
| Thank You | `submit/submit.html` | Confirmation after submitting ("Thank You for Approaching Us"), with a link back home |
| Doctors | `doctors/dotors.html` | Available doctors with specialty, experience and consultation hours |
| Gallery | `gallery/gallery.html` | Doctors with patient success stories, partner hospitals, and trainers |
| Hospitals | `hospitals/hospitals.html` | Hospitals near you and their specialties/facilities |
| Schools | `schools/schools.html` | Medical schools offering training programmes |
| My Profile | `my profile/profil.html` | User menu (edit name, edit contact number, help & support) |

> All doctor, hospital and school entries are **sample/placeholder content** for the prototype.

## 🛠️ Tech Stack

Plain **HTML5 + CSS3**: one stylesheet per page, no JavaScript and no build step.

## 📸 Screenshots

<!-- [TODO: add screenshots of the home page and the consultation form] -->
| Home | Get Started | Doctors |
| --- | --- | --- |
| ![](docs/home.png) | ![](docs/get-started.png) | ![](docs/doctors.png) |

## 🚀 Running Locally

The site is static, so any local web server works. Easiest option: serve the `wp clone web` folder:

```bash
cd "wp clone web"
python -m http.server 5500
# open http://127.0.0.1:5500/first%20pg/yourdoctor.html
```

You can also open `wp clone web/first pg/yourdoctor.html` directly in a browser. Page links and assets use relative paths, so navigation works from the filesystem and from a static host.

## 📁 Project Structure

```
wp clone web/
├── first pg/        # home page (yourdoctor.html) + images + style.css
├── get started/     # consultation form
├── submit/          # thank-you page
├── doctors/         # doctors listing
├── gallery/         # success stories, partner hospitals, and trainers
├── hospitals/       # hospitals listing
├── schools/         # training schools listing
└── my profile/      # user menu
```

## 🗺️ Ideas for next steps

- Add a root `index.html` that points at the home page, so the GitHub Pages root opens the landing page, and rename folders to drop spaces (`first-pg`, `get-started`, `my-profile`)
- Make the consultation form actually submit (e.g. Formspree or a small backend)
- Responsive layout review and accessibility pass (alt text, contrast, keyboard navigation). These matter especially for an audience with disabilities

## 📄 License

[TODO: choose a licence]
