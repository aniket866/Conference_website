## 🧾 Description

This PR implements a dedicated logout action across the Navbar and Admin UI. It ensures that the authentication token and user information (name, photo) are cleared from `localStorage` upon logout, and the user is redirected to the `/login` page. It also fixes a bug in the Navbar's prop handling that prevented it from updating its authentication state in real-time.

## 🧩 Type of change

- [x] Bug fix (non-breaking)
- [x] New feature (non-breaking)
- [ ] Breaking change
- [ ] Documentation update
- [ ] Refactor / maintenance

## 🧪 How to test

List the exact steps/commands to verify the change:

- [ ] Backend: `npm start`
- [x] Frontend: `npm run dev`
- [ ] API: call endpoint(s) affected

Steps:
1. Log in as an admin via `/login`.
2. Observe the "Admin" and "Logout" buttons appearing in the Navbar.
3. Click "Logout" from the Navbar or the Admin Panel top bar.
4. Verify that you are redirected to `/login` and that `localStorage` items (`token`, `name`, `photo`) are cleared.
5. Verify that the "Admin" and "Logout" buttons are no longer visible in the Navbar.

## 📸 Screenshots

Add screenshots as proof of changes:

- [ ] Before screenshot
- [ ] After screenshot

## ✅ Checklist

- [x] I ran the app locally and verified the change
- [ ] I updated documentation when needed
- [x] I did a self-review
- [ ] I didn’t include secrets in commits
