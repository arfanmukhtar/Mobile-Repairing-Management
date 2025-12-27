# 🚀 QUICK START GUIDE - Mobile Repair System

## What You Have

A complete Laravel + React application for managing mobile repair shops with:
- Owner dashboard for managing multiple shops and managers
- Manager dashboard for handling customers and repair bookings
- Full authentication system
- Database schema and migrations
- Modern React UI with Tailwind CSS
-  Repair and Order Booking
-  Add search functionality
-  Implement pagination
-  Add validation messages
-  Dashboard statistics/charts
-  Email notifications and Email Campaigns
-  Real-time updates
-  SMS notifications
-  Mobile app
-  Advanced reporting
-  Reports

---



## ⚡ Installation (5 Minutes)

### 1. Extract Files
```bash
# If you have a zip file
unzip mobile-repair-system.zip
cd mobile-repair-system
```

### 2. Install Dependencies
```bash
composer install
npm install
```

### 3. Environment Setup
```bash
cp .env.example .env
php artisan key:generate
```

Edit `.env` - Update these lines:
```env
DB_DATABASE=mobile_repair_system
DB_USERNAME=root
DB_PASSWORD=your_password
```

### 4. Create Database
```bash
# MySQL command line
mysql -u root -p
CREATE DATABASE mobile_repair_system;
EXIT;

# Or use the provided SQL file
mysql -u root -p < database/mobile_repair_system.sql
```

### 5. Run Migrations
```bash
php artisan migrate
```

### 6. Start Development
```bash
# Terminal 1
npm run dev

# Terminal 2
php artisan serve
```

### 7. Open Browser
Visit: `http://localhost:8000`

---

## 🎯 First Steps

1. **Register an Owner Account**
   - Click "Register Your Shop"
   - Fill in your details
   - You'll be redirected to the owner dashboard

2. **Add Your First Shop**
   - Click "Shops" in navigation
   - Click "Add New Shop"
   - Fill in shop details

3. **Create a Manager**
   - Click "Managers" in navigation
   - Click "Add New Manager"
   - Assign them to a shop

4. **Test Manager Login**
   - Logout
   - Login with manager credentials
   - See manager dashboard

---

## 🔧 Common Issues & Fixes

### Issue: Composer not found
```bash
# Install composer
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
```

### Issue: npm install fails
```bash
rm -rf node_modules package-lock.json
npm cache clean --force
npm install
```

### Issue: Database connection error
- Check MySQL is running: `sudo service mysql status`
- Verify credentials in `.env`
- Test: `php artisan migrate:status`

### Issue: 404 on all pages
```bash
php artisan route:clear
php artisan cache:clear
php artisan config:clear
```

### Issue: Blank page
- Check browser console for errors
- Make sure `npm run dev` is running
- Clear browser cache

---



## 📚 Learning Resources

- Laravel: https://laravel.com/docs
- React: https://react.dev
- Inertia.js: https://inertiajs.com
- Tailwind CSS: https://tailwindcss.com

---

## ⚠️ Important Notes

1. **Never commit `.env`** - It contains sensitive data
2. **Run migrations** before starting
3. **Keep `npm run dev` running** during development
4. **Use `npm run build`** for production
5. **Clear cache** after config changes

---

## ✅ Success Checklist

- [ ] All dependencies installed
- [ ] Database created and migrated
- [ ] Both terminals running (npm & php artisan)
- [ ] Landing page loads at localhost:8000
- [ ] Can register an owner account
- [ ] Can create a shop
- [ ] Can create a manager
- [ ] Manager can login
- [ ] Manager can create bookings

---

## 🎉 You're Ready!
Your mobile repair booking system is ready to use. Start by registering an owner account and exploring the features!

For detailed documentation, see:
- README.md - Overview

Happy coding! 🚀

# Buy Now 
Email: arfan67@gmail.com

