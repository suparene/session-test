# Session test

Demonstrate session expiration

# Preparation

Create a user: \
In project's `Dashboard > Authentication > Users` click `Add user`, and select `Add a new user`.\

Fill in new user details, e.g. :

```
Email address: user@example.com
User Password: secret
Auto confirm user? = SELECTED
```

From `Project settings > General`, copy `Project ID`. \
From `Project settings > API Keys`, copy default `Publishable key`.\
Store both values in the `session-test.html` file:

```js
    const project_id = 'abcd...'
    const publishable_key = 'sb_publishable_...'
```

Serve with e.g. :

```sh
python3 -m http.server 8000
```

and load `localhost:8000/session-test.html` in browser.
