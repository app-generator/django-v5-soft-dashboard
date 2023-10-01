# Django v5 [Soft Dashboard](https://appseed.us/product/soft-ui-dashboard/django/)

Open-source **Django** project crafted on top of **[Soft UI Dashboard](https://appseed.us/product/soft-ui-dashboard/django/)**, an open-source `Bootstrap 5` design from `Creative-Tim`.
Designed for those who like bold elements and beautiful websites. Made of hundreds of elements, designed blocks and fully coded pages, `Soft UI Dashboard` is ready to help you create stunning websites and web apps.

- 👉 Read more about **[Django 5 Release Highlights](https://blog.appseed.us/django-5-release-summary-and-sample/)**
- 🚀 See more **[Open-source and Free Django 5 Starters](https://github.com/app-generator/django-5-release-free-samples)**  

<br />

> Features: 

- ✅ `Up-to-date Dependencies` - **Django v5.x**
- ✅ Theme: [Django Admin Soft](https://github.com/app-generator/django-admin-soft-dashboard), designed by [Creative-Tim](https://www.creative-tim.com/product/soft-ui-dashboard?AFFILIATE=128200)
  - `can be used in any Django project` (new or legacy)
- ✅ **Authentication**: `Django.contrib.AUTH`, Registration
- 🚀 `Deployment` 
  - `CI/CD` flow via `Render`
  - [Django Soft - Go LIVE](https://www.youtube.com/watch?v=1QVdQVSkUCI) - `video presentation`

<br />

![Django Admin Soft - Template project for Django provided by AppSeed.](https://user-images.githubusercontent.com/51070104/215729207-5cce250e-54da-4712-89a9-c1fd6b0a149e.png)

<br />

## Manual Build 

> 👉 Download the code  

```bash
$ git clone https://github.com/app-generator/django-v5-soft-dashboard.git
$ cd django-v5-soft-dashboard
```

<br />

> 👉 Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip install -r requirements.txt
```

<br />

> 👉 Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> 👉 Create the Superuser

```bash
$ python manage.py createsuperuser
```

<br />

> 👉 Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

## **Deploy on Render**

- Create a Blueprint instance
  - Go to https://dashboard.render.com/blueprints this link.
- Click `New Blueprint Instance` button.
- Connect your `repo` which you want to deploy.
- Fill the `Service Group Name` and click on the `Update Existing Resources` button.
- Edit the Environment and [specify the PYTHON_VERSION](https://render.com/docs/python-version)
  - Version `3.11.5` was used for **[this deployment](https://django-v5-datta.onrender.com/)**
- After that, your deployment will start automatically.

At this point, the product should be LIVE.

<br />

## Codebase structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                            
   |    |-- settings.py   # Project Configuration  
   |    |-- urls.py       # Project Routing
   |
   |-- home/
   |    |-- views.py      # APP Views 
   |    |-- urls.py       # APP Routing
   |    |-- models.py     # APP Models 
   |    |-- tests.py      # Tests  
   |     
   |-- templates/
   |    |-- includes/     # UI components 
   |    |-- layouts/      # Masterpages
   |    |-- pages/        # Kit pages 
   |
   |-- static/   
   |    |-- css/                                   # CSS Files 
   |    |-- scss/                                  # SCSS Files 
   |         |-- soft-ui-dashboard/_variables.scss # File Used for Theme Styling
   |
   |-- requirements.txt   # Project Dependencies
   |
   |-- env.sample         # ENV Configuration (default values)
   |-- manage.py          # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />

## Recompile SCSS  

The SCSS/CSS files used to style the Ui are saved in the `static` directory. 
In order to update the Ui colors (primary, secondary) this procedure needs to be followed. 

```bash
$ yarn                                             # install modules
$ vi static/scss/soft-ui-dashboard/_variables.scss # edit variables 
$ gulp                                             # SCSS to CSS translation
```

The `_variables.scss` content defines the `primary` and `secondary` colors: 

```scss
$primary:       #cb0c9f !default;   // EDIT for customization 
$secondary:     #8392AB !default;   // EDIT for customization 
$info:          #17c1e8 !default;   // EDIT for customization 
$success:       #82d616 !default;   // EDIT for customization 
$warning:       #fbcf33 !default;   // EDIT for customization 
$danger:        #ea0606 !default;   // EDIT for customization 
```

<br />

## [Django Soft Dashboard](https://appseed.us/product/soft-ui-dashboard-pro/django/) `PRO`

This design is a pixel-perfect [Bootstrap 5](https://www.admin-dashboards.com/bootstrap-5-templates/) Dashboard with a fresh, new design concept. `Soft UI Dashboard PRO` is built with over 300 frontend individual elements, like buttons, inputs, navbars, nav tabs, cards, or alerts, giving you the freedom of choosing and combining.

> Features: 

- `Up-to-date Dependencies`
- `Design`: [Django Theme Soft PRO](https://github.com/app-generator/django-admin-soft-pro) - `PRO Version`
- `Sections` covered by the design:
  - **Admin section** (reserved for superusers)
  - **Authentication**: `Django.contrib.AUTH`, Registration
  - **All Pages** available in for ordinary users 
- `Docker`, `Deployment`:
  - `CI/CD` flow via `Render`

<br />

![Soft UI Dashboard Pro](https://user-images.githubusercontent.com/51070104/211278814-881e0fcf-7986-4386-afee-540aa0f53bba.png)

<br />

---
[Django Soft Dashboard](https://appseed.us/product/soft-ui-dashboard/django/) - **Django** starter provided by **[AppSeed](https://appseed.us/)**
