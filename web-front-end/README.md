# Frontend

This contains the files for the webpage. This contains a basic login modal and a register modal.

## How to run

You can run a live server extension from your VS Code.

### If you did not install Live Server in your VSCode previously, you will need to do so as explained below. 

In your left sidebar, click on the extensions icon and search for Live Server.

This extension allows us to serve the HTML file to the internet browser. Next, open "index.html" and run the file with Live Server. If you are not able to see the "Run with Live Server" option on the bottom right corner of the code editor, you should be able to see a "Go Live" button. Click on the button and and within your internet browser, you should be redirected to http://127.0.0.1:5500. You should see the image as shown below.

☁️ Note: For users of a cloud development environment, look for the Go Live button at the bottom right corner of your window and click on it. You will then be redirected to a file explorer. Navigate to the pages folder which should then open to your index page. The URL might look something like this: https://ideal-invention-wrv446wvrqx2jrv-5500.app.github.dev/authentication-and-authorisation-with-expressjs/web-front-end/pages/.

You will also need to make edits to the following files to account for your environment's public URL, in place of 127.0.0.1:4001:

- index.html line 28

- profile.html lines 28 and 47

- register.html line 34

- admin/dasboard.html line 26

- admin/user.html lines 32 and 55
Important: Then set your forwarded address from Private to Public

> [!NOTE]
> If you are using GitHub Codespaces, Gitpod or similar, those URLs might be redirected in VSCode Web (or VSCode desktop). You should check the **Ports** tab of your editor. Your URL
> http://localhost:5500 might be redirected to something like http://orange-marmalade.github.codespace.dev (not a real link). If it is set to private while running, please set it to
> Public by right-clicking the row of where the redirected URL is.

Make sure the backend is running. Instructions to run the backend is located at the `back-end` directory's `README.md`.

## File Structure

```
.
└── .
    ├── index.html
    ├── js
    │   ├── README.md
    │   └── scripts.js
    ├── pages
    │   ├── profile.html
    │   └── register.html
    ├── README.md
    └── styles
        └── styles.css

Note: Not all files are indicated
```

The `index.html` file is where the login logic resides. The `profile.html` file is where the profile section resides. The `register.html` is where the register logic resides.
We also have `style.css` which contains the styling of our modals. Combining all this, the `scripts.js` allows the frontend to communicate with the backend such as

- authentication logins
- registration
- routing
