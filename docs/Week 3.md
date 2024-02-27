
# Week 3: From March 11 to March 15

# Chapter 6: Authentication and database (security, data persistence)
 
## <div style="color: Royalblue;"> Table of contents </div>

- Authentication: user registration, hash with bcrypt
- Connecting a MySQL database to a Node.js application
- Executing SQL queries on a MySQL database with NodeJS
- Using a MySQL database in NodeJS with Sequelize

## <div style="color: Royalblue;">Authentication: user registration, hash with bcrypt</div>

The purpose of authentication is to be able to know who is a user<br>

- The purpose of authorization is to:

- authorize or deny an action

- log who initiated the action

- First and foremost: NEVER store a password in clear text in a database

- plaintext = readable, without having passed through a hash mechanism

- Authentication to a web site involves sessions, which work thanks to cookies
stored on the user's computer

- When the user enters his login and password, it is verified that he is a user.
login and password are identical

- If necessary, we associate the user id with the session:
`req.session.userId = user.id`

- When the user registers, we check that no other user has the same e-mail address, to avoid collisions.
- Next, we hash the password, generally using the bcrypt module
- We store the email and password in their hashed form in the database
- When the user logs in, we retrieve the entry in the database with the identical email address
- Next, we use the function bcrypt.compare(mdpForm, mdpHashéEnBDD)
- This asynchronous function returns true if the two passwords are identical, false otherwise:

```js linenums="1"
if (await bcrypt.compare(mdpForm, mdpHasheBDD)) {
// congrats
} else {
// go out !
}
```