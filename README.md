# myISA: My Intelligent Study Assistant

Welcome to the **myISA** repository! This project is a landing page for **myISA**, an intelligent study assistant designed to help students enhance their learning experience with personalized tools and features.

## Features

The landing page highlights the key features of myISA, including:

- **Personalized Study Plans**: Generate study plans tailored to individual goals and progress.
- **Summarize Readings**: Upload readings or textbooks to generate concise summaries.
- **Study On The Go**: Interact with myISA using voice-based questions about class material.
- **LMS Integration**: Seamlessly integrate with platforms like Canvas or Google Classroom.
- **Adaptive Learning Modules**: Assign modules tailored to individual student needs.
- **Reminders & Deadlines**: Stay organized with reminders for exams, assignments, and deadlines.

## Latest Posts

The page also includes a section for the latest posts, such as updates on new features or educational content.

---

## Repository Structure

This repository includes the following key directories and files:

- `assets/`: Contains images, icons, and other assets used in the project.
- `content/`: Stores content files for the site.
- `layouts/`: Includes layout templates for different sections of the site.
- `static/`: Contains static files like CSS, JavaScript, and additional assets.
- `themes/`: Holds theme-related files.
- `config.toml`: Configuration file for the Hugo static site generator.
- `publish_to_gh_pages.sh`: Script to deploy the site to GitHub Pages.

---

## Deployment

This project is deployed using **GitHub Pages**. To view the live site, visit:

[myISA Landing Page](https://muditm006.github.io/hugo-mock-landing-page/)

---

## How to Run Locally

To run this project locally:

1. Clone this repository:
git clone https://github.com/muditm006/hugo-mock-landing-page.git
2. Navigate to the project directory:
cd hugo-mock-landing-page
3. Install [Hugo](https://gohugo.io/) if you haven't already.
4. Run the local development server:
hugo server -D
5. Open your browser and navigate to `http://localhost:1313`.

---

## GitHub Actions Workflow: Build and Deploy Hugo Website

This repository includes an integrated GitHub Actions workflow that automates the deployment process. The workflow is triggered on every push to the `main` branch and performs the following steps:

1. **Check Out Source Repository**:
- Uses `actions/checkout@v3.5.1` to fetch the repository, including submodules and full commit history.

2. **Initialize Hugo Environment**:
- Sets up Hugo using `peaceiris/actions-hugo@v2.6.0`, specifying version `0.144.1` with extended support enabled.

3. **Compile Hugo Static Files**:
- Runs Hugo with flags for draft content (`-D`), garbage collection (`--gc`), and minification (`--minify`).

4. **Publish to GitHub Pages**:
- Deploys the generated static files to the `gh-pages` branch using `peaceiris/actions-gh-pages@v3.9.3`.

This automated CI/CD pipeline ensures that any changes pushed to the repository are immediately reflected on the live site hosted via GitHub Pages.
