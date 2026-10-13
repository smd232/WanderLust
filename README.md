[README.md](https://github.com/user-attachments/files/32622846/README.md)
# 🌍 WanderLust

A full-stack travel and stay booking web app. Browse listings, view them on an interactive map, upload photos, and manage your own listings with secure user accounts.

<!-- Add a screenshot or GIF of your homepage here -->
<!-- ![WanderLust Screenshot](./public/screenshots/home.png) -->

---

## ✨ Features

- **User authentication** – sign up, log in and log out with secure sessions (Passport.js)
- **Listings** – create, view, edit and delete travel/stay listings
- **Image uploads** – photos stored in the cloud with Cloudinary
- **Interactive maps** – listing locations powered by Mapbox
- **Validation** – server-side schema validation with Joi
- **Flash messages** – clear success and error feedback
- **Persistent sessions** – session data stored in MongoDB
- **Clean, minimal UI** – server-rendered EJS templates with reusable layouts

---

## 🛠️ Tech Stack

| Layer | Technology |
| --- | --- |
| Runtime | Node.js |
| Framework | Express.js |
| Database | MongoDB with Mongoose |
| Templating | EJS, EJS-Mate |
| Authentication | Passport, passport-local, passport-local-mongoose |
| File uploads | Multer, Cloudinary, multer-storage-cloudinary |
| Maps / Geocoding | Mapbox SDK |
| Validation | Joi |
| Sessions | express-session, connect-mongo, connect-flash |

---

## 📁 Project Structure


├── controllers/     # Route handler logic
├── init/            # Database seed / initialization data
├── models/          # Mongoose schemas and models
├── public/          # Static assets (CSS, JS, images)
├── routes/          # Express route definitions
├── utils/           # Helper utilities (e.g. error handling)
├── views/           # EJS templates
├── app.js           # Application entry point
├── cloudConfig.js   # Cloudinary configuration
├── authMiddleware.js    # Custom middleware (auth, validation)
└── schema.js        # Joi validation schemas

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v21.5.0 recommended)
- A [MongoDB](https://www.mongodb.com/) database (local or MongoDB Atlas)
- A [Cloudinary](https://cloudinary.com/) account
- A [Mapbox](https://www.mapbox.com/) access token

### Installation

bash
# Clone the repository
git clone https://github.com/smd232/Project.git

# Move into the project folder
cd Project

# Install dependencies
npm install

### Environment Variables

Create a `.env` file in the root directory and add your own keys:

env
CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret
MAP_TOKEN=your_mapbox_access_token
ATLASDB_URL=your_mongodb_connection_string
SECRET=your_session_secret

> ⚠️ Never commit your `.env` file. It is already excluded via `.gitignore`.

### Run the App

bash
node app.js


Then open [http://localhost:8080](http://localhost:8080) in your browser.

---

## 🗺️ Roadmap

- [ ] Full "All Packages" listings page
- [ ] Reviews and star ratings
- [ ] Favorites / wishlist
- [ ] Search and filters
- [ ] Booking flow and payments

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m "Add amazing feature"`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the ISC License.

---

## 👩‍💻 Author

**Syeda Maryam** – [@smd232](https://github.com/smd232)

Project link: [https://github.com/smd232/Project](https://github.com/smd232/Project)
