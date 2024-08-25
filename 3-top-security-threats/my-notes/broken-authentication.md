# Broken Authentication - hashing password

How to hash password in Node Express application.

## YouTube Training

[Hashing with bcrypt](https://youtu.be/AzA_LTDoFqY?si=KzOvA0yTdgf7r9Be) on YouTube.

1. Create a 'app.js; code file.
2. Write import state to import the bcrypt library.
3. Define a `password` variable object and assign it a String value of an example password.
4. To hash that password simply define a `hash` variable and assign the `bcrypt` as an async `await` method, and pass in two paramenters - the `password` object and the number value of `10`.
5. To test this two new objects we need to write the console log statement and pass in an object value of the two objects we defined earlier on.
6. In the Terminal, run this script using `$ node app.js` .
7. Now we can see the value of the password and the value of the hash is a very long messing string which we store in the DB and if cyber criminals get access to our database they will get this messy string rather than the user's password of plain text password.
8. Also, a developer with too high privilages will not see the plain text password but the long messy string.

### Conclusion

During my next Backend development project I will be using this 'Hashing with bcrypt' technique to protect the user's password.
