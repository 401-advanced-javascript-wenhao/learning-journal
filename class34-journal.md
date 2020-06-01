# Class 34 - `<Login />` and `<Auth \>` - 5/29/2020

* Authentication - valid user is logged in  
* Authorization - what permissions does the user have 
* Combine Authentication and Authorization to create UI that ensures that users only have access to content and functionality that they are granted access to 

## Example: 
```javascript
// state  
this.state = {
  loggedIn: false,
  login: this.login,
  logout: this.logout,
  token: null,
  user: {}
};

// methods in the context
login = (username, password) => {
  fetch(`${API}/signin`, {
    method: 'post',
    mode: 'cors',
    cache: 'no-cache',
    headers: new Headers({
      'Authorization': `Basic ${btoa(`${username}:${password}`)}`
    })
  })
  .then(data => data.text())
  .then(token => this.validateToken(token))
  .catch(err => console.error(err));
}

validateToken = token => {
  try {
    let user = jwt.verify(token, 'supersecret');
    this.setLoginState(true, token, user);
  } catch(err) {
    this.setLoginState(false, null, {})
  }
}

setLoginState = (loggedIn, token, user) => {
  cookie.save('auth', token);
  this.setState({token, loggedIn, user});
}

logout = () => {
  this.setLoginState(false, null, {});
}
```