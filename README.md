# Certificate Project

A responsive certificate generation system for training completion certificates.

## Features

- **Dynamic Certificate Generation**: Supports multiple people with different certificate data
- **Responsive Design**: Works on desktop and mobile devices
- **Dual Language**: English and Thai sections
- **Easy to Update**: Simply edit `data.js` to add more people

## How to Use

### View Certificates

Open `index.html` in a web browser. Use the navigation buttons to switch between different people's certificates.

You can also use URL parameters:
- `index.html?id=1` - First person
- `index.html?id=2` - Second person
- `index.html?id=3` - Third person

### Add More People

Edit the `data.js` file and add new entries to the `certificateData` array:

```javascript
{
    id: 4,
    name: "ชื่อผู้ได้รับ",
    certNumber: "รหัสใบรับรอง",
    course: "ชื่อหลักสูตร",
    duration: "ระยะเวลา",
    trainingDate: "วันที่อบรม",
    betweenDate: "ระหว่างวันที่",
    issueDate: "วันที่ออกใบรับรอง",
    issueFullDate: "วันที่ออกใบรับรองแบบเต็ม"
}
```

## Files

- `index.html` - Main HTML file
- `style.css` - Stylesheet
- `data.js` - Certificate data for all people
- `cer_bg.png` - Background image for English section
- `logo.png` - Company logo

## Technologies

- HTML5
- CSS3 (with responsive design)
- Vanilla JavaScript
- Google Fonts (Sarabun)

## Deploying to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right and select "New repository"
3. Name your repository (e.g., `certificate`)
4. Choose "Public" visibility
5. Do NOT initialize with README (we already have one)
6. Click "Create repository"

### Step 2: Push Code to GitHub

Run these commands in the `/home/x/certificate` directory:

```bash
# Add all files to git
git add .

# Commit the files
git commit -m "Initial commit: Certificate system with 3 people"

# Add your GitHub repository as remote (replace USERNAME with your GitHub username)
git remote add origin https://github.com/USERNAME/certificate.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait a few minutes for deployment

### Step 4: Access Your Certificates

Your certificates will be available at:
- `https://USERNAME.github.io/certificate/` (Person 1)
- `https://USERNAME.github.io/certificate/?id=2` (Person 2)
- `https://USERNAME.github.io/certificate/?id=3` (Person 3)

Replace `USERNAME` with your actual GitHub username.

### Example URLs

If your GitHub username is `john-doe`:
- Person 1: `https://john-doe.github.io/certificate/`
- Person 2: `https://john-doe.github.io/certificate/?id=2`
- Person 3: `https://john-doe.github.io/certificate/?id=3`
