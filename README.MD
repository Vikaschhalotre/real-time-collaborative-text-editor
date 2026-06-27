# Collaborative Text Editor

A real-time collaborative rich text editor that allows multiple users to edit the same document simultaneously. The project uses Django Channels, WebSockets, Redis, Yjs (CRDT), and React to provide instant synchronization between connected users.

![demo](demo.gif)

Made using:

- Django
- Django Channels
- Redis
- Vite React
- Yjs
- Remirror

## Features:

- Real-time collaboration editing
- Uses data-types like CRDTs to avoid conflicts
- Uses Vite React for faster development & interactive user experience
- Other users can see the changes in real-time + the cursor position of the user who is typing

There are some more features which can be added, and to leave space for that, I have created the project using Django as the backend.

## Installation:

1. Fork the repo
2. Clone the repo: `$ git clone`
3. **For backend:**
   - `cd` into `app-server`
   - Create a virtual environment: `$ python3 -m venv env`
   - Activate the virtual environment: `$ source env/bin/activate`
   - Install the dependencies: `$ pip install -r requirements.txt`
   - Create a `.env` file.
   - Make migrations: `$ python manage.py makemigrations`
   - Migrate: `$ python manage.py migrate`
   - If you want to spin up redis server using docker: `$ docker run -p 6379:6379 -d redis:5`
   - Run the server: `$ python manage.py runserver`
4. **For frontend:**
   - `cd` into `app`
   - Run `yarn install` or `npm install`
   - Run `yarn dev` or `npm run dev`
   
🚀 Running the Project

Backend

http://127.0.0.1:8000

Frontend

http://localhost:5173

- Open the application in two browser windows and start typing to experience real-time collaboration.

## Future plans

- [ ] Optimize backend
- [ ] Optimize frontend
- [ ] Use peer-to-peer communication using WebRTC
- [ ] Add ability to create multiple documents(or rooms)

- Authentication
- Multiple documents
- Shareable document links
- User roles & permissions
- Persistent document storage
- Docker Compose support


With these features in mind, this project can be a great starting point for anyone who wants to build a real-time collaborative editor or take this knowledge and apply it to their own projects.

## Contributing

Contributions are welcome! Fork the repo and submit a pull request. If you have any questions, feel free to open an issue.

Made with :heart: by [Vikas](https://github.com/Vikaschhalotre)
