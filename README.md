# VA Portfolio

A modern, responsive portfolio website built with Django for Arison Gift, a professional Social Media Manager specializing in social media management, marketing, and email marketing services.

## 🚀 Features

- **Single-Page Design**: Smooth scrolling navigation with distinct sections
- **Responsive Layout**: Optimized for desktop, tablet, and mobile devices
- **SEO Optimized**: Comprehensive meta tags for better search engine visibility
- **Social Media Integration**: Links to professional social media profiles
- **Portfolio Showcase**: Display of projects and client testimonials
- **Contact Integration**: Direct email and phone contact options
- **CV Download**: Easy access to downloadable resume
- **Dark/Light Theme Support**: Modern design with accessibility considerations

## 📋 Sections

- **Intro**: Hero section with professional introduction
- **About**: Personal background and mission statement
- **Services**: Detailed service offerings (Social Media Management, Marketing, Email Marketing)
- **Experience**: Professional background and tools used
- **Works**: Portfolio of completed projects with images
- **Testimonials**: Client reviews and feedback
- **Contact**: Contact information and social media links

## 🛠 Tech Stack

- **Backend**: Django 4.x
- **Frontend**: HTML5, CSS3, JavaScript
- **Styling**: Custom CSS with vendor styles
- **Icons**: SVG icons for social media
- **Deployment**: Heroku-ready with Gunicorn

## 📦 Installation

### Prerequisites
- Python 3.8+
- pip
- Git

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/va-portfolio.git
   cd va-portfolio
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Apply migrations**
   ```bash
   python manage.py migrate
   ```

5. **Collect static files**
   ```bash
   python manage.py collectstatic --noinput
   ```

6. **Run the development server**
   ```bash
   python manage.py runserver
   ```

7. **Open your browser** and navigate to `http://127.0.0.1:8000/`

## 🚀 Deployment

### Heroku Deployment

1. **Install Heroku CLI** and login
   ```bash
   heroku login
   ```

2. **Create a new Heroku app**
   ```bash
   heroku create your-app-name
   ```

3. **Set environment variables** (if needed)
   ```bash
   heroku config:set DEBUG=False
   ```

4. **Deploy**
   ```bash
   git push heroku main
   ```

5. **Run migrations on Heroku**
   ```bash
   heroku run python manage.py migrate
   ```

6. **Collect static files on Heroku**
   ```bash
   heroku run python manage.py collectstatic --noinput
   ```

## 📁 Project Structure

```
va-portfolio/
├── config/                 # Django project settings
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── portfolio/              # Main Django app
│   ├── base/               # Portfolio app
│   │   ├── templates/
│   │   │   └── base/
│   │   │       └── index.html
│   │   ├── static/         # Static files
│   │   │   ├── css/
│   │   │   ├── js/
│   │   │   ├── images/
│   │   │   └── cv/
│   │   └── views.py
├── Procfile               # Heroku deployment file
├── requirements.txt       # Python dependencies
├── manage.py
└── README.md
```

## 🎨 Customization

### Content Updates
- Edit `portfolio/base/templates/base/index.html` to modify content
- Update images in `portfolio/static/images/`
- Replace CV file in `portfolio/static/cv/`

### Styling
- Main styles: `portfolio/static/css/styles.css`
- Vendor styles: `portfolio/static/css/vendor.css`

### Adding New Sections
1. Add HTML structure in the template
2. Update navigation links
3. Add corresponding CSS styles

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Arison Gift**
- Email: arisongift25@gmail.com
- Phone: (+234) 810 882 6448
- LinkedIn: [Arison Gift](https://www.linkedin.com/in/arison-gift-935515372)
- Portfolio: [View Live Site](https://your-deployed-site.com)

## 🙏 Acknowledgments

- Built with [Django](https://www.djangoproject.com/)
- Icons from various open-source libraries
- Inspired by modern portfolio designs

---

⭐ If you find this project helpful, please give it a star!
