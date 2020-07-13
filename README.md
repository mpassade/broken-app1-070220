### Broken App Corrections
* At app.js line 21 changed proces.env.MONGODB_URI to process.env.MONGODB_URI
* Added module.exports = mongoose.model('User', UserSchema) to the end of User.js
* Added async to line 6 in userController.js
* Set variables equal to req.body at line 11 un userController.js
* In index.js line 6, rendered 'main/home' instead of 'home'
* Changed userRoutes.js line 66 to '/login',
* In userRoutes.js line 67 changed 'local' to 'local-login'
* Added const bcrypt = require('bcryptjs') to User.js line 3
* In userRoutes.js at line 68, changed successRedirect route to '/home'
* In userRoutes.js at line 69, changed failureRedirect route to '/api/users/login'
* Removed ", { errors: req.flash('errors') }" from line 62 in userRoutes.js
* Removed ", { errors: req.flash('errors') }" from line 35 in userRoutes.js
* In userRoutes.js line 59, changed the return to res.redirect('/')
* In app.js, moved the flash, passport initialize, and passport session middleware below the session middleware
* In app.js moved the router middleware and mongoose connection to the bottom of the page before module.exports
* In userController.js line 79, capitalized p in userpassword