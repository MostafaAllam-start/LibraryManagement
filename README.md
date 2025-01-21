<div align="left" style="position: relative;">
<h1>Library Management Project</h1>
<p align="left">
	<em><code>❯ This project is the final project for the training of ITI fullstack python track</code></em>
</p>
<p align="left">
	<img src="https://img.shields.io/github/license/MostafaAllam-start/LibraryManagement?style=default&logo=opensourceinitiative&logoColor=white&color=0080ff" alt="license">
	<img src="https://img.shields.io/github/last-commit/MostafaAllam-start/LibraryManagement?style=default&logo=git&logoColor=white&color=0080ff" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/MostafaAllam-start/LibraryManagement?style=default&color=0080ff" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/MostafaAllam-start/LibraryManagement?style=default&color=0080ff" alt="repo-language-count">
</p>
<p align="left"><!-- default option, no dependency badges. -->
</p>
<p align="left">
	<!-- default option, no dependency badges. -->
</p>
</div>
<br clear="right">

##  Table of Contents

- [ Overview](#-overview)
- [ Features](#-features)
- [ Project Structure](#-project-structure)
  - [ Project Index](#-project-index)
- [ Getting Started](#-getting-started)
  - [ Prerequisites](#-prerequisites)
  - [ Installation](#-installation)
  - [ Usage](#-usage)
  - [ Testing](#-testing)
- [ Contributing](#-contributing)
- [ Acknowledgments](#-acknowledgments)

---

##  Overview

<code>❯Developed a web application for managing a library system, allowing users to manage books, borrowers, and transactions seamlessly.</code>

---

##  Features

- **Admin CRUD operations for managing books, members, and borrowing records.**
- **User authentication and role-based access control for administrators and users.**
- **Search functionality for books and members with filters and sorting options.**
- **Notification system for overdue books and return reminders.**
- **Optimized database queries for enhanced performance.**

---

##  Project Structure

```sh
└── LibraryManagement/
    ├── Admin
    │   ├── __init__.py
    │   ├── admin.py
    │   ├── apps.py
    │   ├── forms.py
    │   ├── migrations
    │   │   └── __init__.py
    │   ├── models.py
    │   ├── templates
    │   │   └── Admin
    │   │       └── admin_dashboard.html
    │   ├── tests.py
    │   ├── urls.py
    │   └── views.py
    ├── Books
    │   ├── __init__.py
    │   ├── admin.py
    │   ├── apps.py
    │   ├── forms.py
    │   ├── migrations
    │   │   ├── 0001_initial.py
    │   │   └── __init__.py
    │   ├── models.py
    │   ├── signals.py
    │   ├── static
    │   │   └── books
    │   │       ├── css
    │   │       │   ├── bootstrap.css
    │   │       │   ├── main.css
    │   │       │   └── vendor.css
    │   │       ├── fonts
    │   │       │   ├── Billy Ohio.eot
    │   │       │   ├── Billy Ohio.woff2
    │   │       │   ├── BillyOhio.svg
    │   │       │   ├── BillyOhio.ttf
    │   │       │   ├── BillyOhio.woff
    │   │       │   ├── Flaticon.eot
    │   │       │   ├── Flaticon.svg
    │   │       │   ├── Flaticon.ttf
    │   │       │   ├── Flaticon.woff
    │   │       │   ├── Flaticon.woff2
    │   │       │   ├── FontAwesome.otf
    │   │       │   ├── flaticon.css
    │   │       │   ├── flaticon.html
    │   │       │   ├── fontawesome-webfont.eot
    │   │       │   ├── fontawesome-webfont.svg
    │   │       │   ├── fontawesome-webfont.ttf
    │   │       │   ├── fontawesome-webfont.woff
    │   │       │   ├── fontawesome-webfont.woff2
    │   │       │   ├── lg.eot
    │   │       │   ├── lg.svg
    │   │       │   ├── lg.ttf
    │   │       │   └── lg.woff
    │   │       ├── images
    │   │       │   ├── Logo.png
    │   │       │   ├── New Logo.png
    │   │       │   ├── cross.png
    │   │       │   ├── favicon.ico
    │   │       │   ├── grid.png
    │   │       │   ├── icon.png
    │   │       │   ├── list.png
    │   │       │   ├── loading.gif
    │   │       │   ├── marker.png
    │   │       │   ├── play.png
    │   │       │   ├── product-03-270x300.jpg
    │   │       │   ├── slider-bg-01.jpg
    │   │       │   ├── slider-bg-02.jpg
    │   │       │   ├── slider-image-01.png
    │   │       │   ├── slider-image-02.png
    │   │       │   ├── video-play.png
    │   │       │   ├── vimeo-play.png
    │   │       │   └── youtube-play.png
    │   │       └── js
    │   │           ├── main.js
    │   │           └── vendor.js
    │   ├── templates
    │   │   └── Books
    │   │       ├── add_author.html
    │   │       ├── author_books.html
    │   │       ├── base.html
    │   │       ├── book_confirm_delete.html
    │   │       ├── book_create_form.html
    │   │       ├── book_list.html
    │   │       ├── book_update_form.html
    │   │       ├── book_update_list.html
    │   │       ├── borrow.html
    │   │       ├── category_books.html
    │   │       ├── category_confirm_delete.html
    │   │       ├── category_create_form.html
    │   │       ├── category_list.html
    │   │       └── category_update_books.html
    │   ├── tests.py
    │   ├── urls.py
    │   └── views.py
    ├── Groups
    │   ├── __init__.py
    │   ├── admin.py
    │   ├── apps.py
    │   ├── migrations
    │   │   └── __init__.py
    │   ├── models.py
    │   ├── tests.py
    │   └── views.py
    ├── MyLibrary
    │   ├── __init__.py
    │   ├── asgi.py
    │   ├── settings.py
    │   ├── urls.py
    │   └── wsgi.py
    ├── Project Sturcture.docx
    ├── Project Sturcture.txt
    ├── README.md
    ├── accounts
    │   ├── __init__.py
    │   ├── admin.py
    │   ├── apps.py
    │   ├── forms.py
    │   ├── migrations
    │   │   ├── 0001_initial.py
    │   │   ├── 0002_rename_image_profile_profile_image.py
    │   │   ├── 0003_alter_profile_profile_image.py
    │   │   ├── 0004_alter_profile_profile_image.py
    │   │   ├── 0005_alter_profile_profile_image.py
    │   │   ├── 0006_alter_profile_profile_image.py
    │   │   ├── 0007_auto_20210923_2319.py
    │   │   ├── 0008_alter_profile_user.py
    │   │   ├── 0009_alter_profile_phone_number.py
    │   │   └── __init__.py
    │   ├── models.py
    │   ├── signals.py
    │   ├── static
    │   │   └── accounts
    │   │       ├── css
    │   │       │   ├── bootstrap.css
    │   │       │   ├── main.css
    │   │       │   └── vendor.css
    │   │       ├── fonts
    │   │       │   ├── Billy Ohio.eot
    │   │       │   ├── Billy Ohio.woff2
    │   │       │   ├── BillyOhio.svg
    │   │       │   ├── BillyOhio.ttf
    │   │       │   ├── BillyOhio.woff
    │   │       │   ├── Flaticon.eot
    │   │       │   ├── Flaticon.svg
    │   │       │   ├── Flaticon.ttf
    │   │       │   ├── Flaticon.woff
    │   │       │   ├── Flaticon.woff2
    │   │       │   ├── FontAwesome.otf
    │   │       │   ├── flaticon.css
    │   │       │   ├── flaticon.html
    │   │       │   ├── fontawesome-webfont.eot
    │   │       │   ├── fontawesome-webfont.svg
    │   │       │   ├── fontawesome-webfont.ttf
    │   │       │   ├── fontawesome-webfont.woff
    │   │       │   ├── fontawesome-webfont.woff2
    │   │       │   ├── lg.eot
    │   │       │   ├── lg.svg
    │   │       │   ├── lg.ttf
    │   │       │   └── lg.woff
    │   │       └── js
    │   │           ├── main.js
    │   │           └── vendor.js
    │   ├── templates
    │   │   ├── base_generic.html
    │   │   ├── contact_us.html
    │   │   ├── profile.html
    │   │   ├── register.html
    │   │   └── registration
    │   │       ├── login.html
    │   │       ├── logout.html
    │   │       ├── password_change_done.html
    │   │       ├── password_change_form.html
    │   │       ├── password_reset_complete.html
    │   │       ├── password_reset_confirm.html
    │   │       ├── password_reset_done.html
    │   │       ├── password_reset_email.html
    │   │       └── password_reset_form.html
    │   ├── tests.py
    │   ├── urls.py
    │   └── views.py
    ├── blog
    │   ├── __init__.py
    │   ├── admin.py
    │   ├── apps.py
    │   ├── forms.py
    │   ├── migrations
    │   │   ├── 0001_initial.py
    │   │   └── __init__.py
    │   ├── models.py
    │   ├── templates
    │   │   └── blog
    │   │       └── blog.html
    │   ├── tests.py
    │   ├── urls.py
    │   └── views.py
    ├── manage.py
    ├── media
    │   ├── book_images
    │   │   ├── 1.1.png
    │   │   ├── 1_translateis_used_to_move_the_selected_element_by_x__y.png
    │   │   ├── Mag.png
    │   │   ├── Mag_TrMGh9A.png
    │   │   ├── Tree_Rules.png
    │   │   ├── background.png
    │   │   ├── background_Pu8EnGL.png
    │   │   └── default.jpg
    │   ├── default.jpg
    │   └── profile_pics
    │       ├── Descendent_selector_is_one_of_many_ways_to_combine_selectors.png
    │       ├── default.jpg
    │       └── default_Qod8myQ.jpg
    └── requirements.txt
```


###  Project Index
<details open>
	<summary><b><code>LIBRARYMANAGEMENT/</code></b></summary>
	<details> <!-- __root__ Submodule -->
		<summary><b>__root__</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Project Sturcture.txt'>Project Sturcture.txt</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/manage.py'>manage.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/requirements.txt'>requirements.txt</a></b></td>
				<td></td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- Books Submodule -->
		<summary><b>Books</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/tests.py'>tests.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/forms.py'>forms.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/views.py'>views.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/apps.py'>apps.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/signals.py'>signals.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/urls.py'>urls.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/admin.py'>admin.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/models.py'>models.py</a></b></td>
				<td></td>
			</tr>
			</table>
			<details>
				<summary><b>templates</b></summary>
				<blockquote>
					<details>
						<summary><b>Books</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/category_update_books.html'>category_update_books.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/borrow.html'>borrow.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/category_books.html'>category_books.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/book_create_form.html'>book_create_form.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/author_books.html'>author_books.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/category_confirm_delete.html'>category_confirm_delete.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/add_author.html'>add_author.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/book_list.html'>book_list.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/category_list.html'>category_list.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/book_update_form.html'>book_update_form.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/book_confirm_delete.html'>book_confirm_delete.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/category_create_form.html'>category_create_form.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/book_update_list.html'>book_update_list.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/templates/Books/base.html'>base.html</a></b></td>
								<td></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>migrations</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Books/migrations/0001_initial.py'>0001_initial.py</a></b></td>
						<td></td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- Admin Submodule -->
		<summary><b>Admin</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/tests.py'>tests.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/forms.py'>forms.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/views.py'>views.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/apps.py'>apps.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/urls.py'>urls.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/admin.py'>admin.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/models.py'>models.py</a></b></td>
				<td></td>
			</tr>
			</table>
			<details>
				<summary><b>templates</b></summary>
				<blockquote>
					<details>
						<summary><b>Admin</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Admin/templates/Admin/admin_dashboard.html'>admin_dashboard.html</a></b></td>
								<td></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- Groups Submodule -->
		<summary><b>Groups</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Groups/tests.py'>tests.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Groups/views.py'>views.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Groups/apps.py'>apps.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Groups/admin.py'>admin.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/Groups/models.py'>models.py</a></b></td>
				<td></td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- accounts Submodule -->
		<summary><b>accounts</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/tests.py'>tests.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/forms.py'>forms.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/views.py'>views.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/apps.py'>apps.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/signals.py'>signals.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/urls.py'>urls.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/admin.py'>admin.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/models.py'>models.py</a></b></td>
				<td></td>
			</tr>
			</table>
			<details>
				<summary><b>templates</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/register.html'>register.html</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/contact_us.html'>contact_us.html</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/base_generic.html'>base_generic.html</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/profile.html'>profile.html</a></b></td>
						<td></td>
					</tr>
					</table>
					<details>
						<summary><b>registration</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/password_change_form.html'>password_change_form.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/password_reset_confirm.html'>password_reset_confirm.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/password_reset_email.html'>password_reset_email.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/password_reset_done.html'>password_reset_done.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/password_reset_form.html'>password_reset_form.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/login.html'>login.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/password_reset_complete.html'>password_reset_complete.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/logout.html'>logout.html</a></b></td>
								<td></td>
							</tr>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/templates/registration/password_change_done.html'>password_change_done.html</a></b></td>
								<td></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>migrations</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0004_alter_profile_profile_image.py'>0004_alter_profile_profile_image.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0001_initial.py'>0001_initial.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0005_alter_profile_profile_image.py'>0005_alter_profile_profile_image.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0009_alter_profile_phone_number.py'>0009_alter_profile_phone_number.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0007_auto_20210923_2319.py'>0007_auto_20210923_2319.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0002_rename_image_profile_profile_image.py'>0002_rename_image_profile_profile_image.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0008_alter_profile_user.py'>0008_alter_profile_user.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0006_alter_profile_profile_image.py'>0006_alter_profile_profile_image.py</a></b></td>
						<td></td>
					</tr>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/accounts/migrations/0003_alter_profile_profile_image.py'>0003_alter_profile_profile_image.py</a></b></td>
						<td></td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
	<details> <!-- MyLibrary Submodule -->
		<summary><b>MyLibrary</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/MyLibrary/settings.py'>settings.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/MyLibrary/urls.py'>urls.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/MyLibrary/asgi.py'>asgi.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/MyLibrary/wsgi.py'>wsgi.py</a></b></td>
				<td></td>
			</tr>
			</table>
		</blockquote>
	</details>
	<details> <!-- blog Submodule -->
		<summary><b>blog</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/tests.py'>tests.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/forms.py'>forms.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/views.py'>views.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/apps.py'>apps.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/urls.py'>urls.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/admin.py'>admin.py</a></b></td>
				<td></td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/models.py'>models.py</a></b></td>
				<td></td>
			</tr>
			</table>
			<details>
				<summary><b>templates</b></summary>
				<blockquote>
					<details>
						<summary><b>blog</b></summary>
						<blockquote>
							<table>
							<tr>
								<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/templates/blog/blog.html'>blog.html</a></b></td>
								<td></td>
							</tr>
							</table>
						</blockquote>
					</details>
				</blockquote>
			</details>
			<details>
				<summary><b>migrations</b></summary>
				<blockquote>
					<table>
					<tr>
						<td><b><a href='https://github.com/MostafaAllam-start/LibraryManagement/blob/master/blog/migrations/0001_initial.py'>0001_initial.py</a></b></td>
						<td></td>
					</tr>
					</table>
				</blockquote>
			</details>
		</blockquote>
	</details>
</details>

---
##  Getting Started

###  Prerequisites

Before getting started with LibraryManagement, ensure your runtime environment meets the following requirements:

- **Programming Language:** Python
- **Package Manager:** Pip


###  Installation

Install LibraryManagement using the following method:

**Build from source:**

1. Clone the LibraryManagement repository:
```sh
❯ git clone https://github.com/MostafaAllam-start/LibraryManagement
```

2. Navigate to the project directory:
```sh
❯ cd LibraryManagement
```

3. Install the project dependencies:


```sh
❯ pip install -r requirements.txt
```




###  Usage
Run LibraryManagement using the following command:

```sh
❯ python manage.py runserver
```


###  Testing
Run the test suite using the following command:

```sh
❯ pytest
```


---

##  Contributing

- **💬 [Join the Discussions](https://github.com/MostafaAllam-start/LibraryManagement/discussions)**: Share your insights, provide feedback, or ask questions.
- **🐛 [Report Issues](https://github.com/MostafaAllam-start/LibraryManagement/issues)**: Submit bugs found or log feature requests for the `LibraryManagement` project.
- **💡 [Submit Pull Requests](https://github.com/MostafaAllam-start/LibraryManagement/blob/main/CONTRIBUTING.md)**: Review open PRs, and submit your own PRs.

<details closed>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**: Start by forking the project repository to your github account.
2. **Clone Locally**: Clone the forked repository to your local machine using a git client.
   ```sh
   git clone https://github.com/MostafaAllam-start/LibraryManagement
   ```
3. **Create a New Branch**: Always work on a new branch, giving it a descriptive name.
   ```sh
   git checkout -b new-feature-x
   ```
4. **Make Your Changes**: Develop and test your changes locally.
5. **Commit Your Changes**: Commit with a clear message describing your updates.
   ```sh
   git commit -m 'Implemented new feature x.'
   ```
6. **Push to github**: Push the changes to your forked repository.
   ```sh
   git push origin new-feature-x
   ```
7. **Submit a Pull Request**: Create a PR against the original project repository. Clearly describe the changes and their motivations.
8. **Review**: Once your PR is reviewed and approved, it will be merged into the main branch. Congratulations on your contribution!
</details>

<details closed>
<summary>Contributor Graph</summary>
<br>
<p align="left">
   <a href="https://github.com{/MostafaAllam-start/LibraryManagement/}graphs/contributors">
      <img src="https://contrib.rocks/image?repo=MostafaAllam-start/LibraryManagement">
   </a>
</p>
</details>

---
