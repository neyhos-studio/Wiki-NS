# Login API

### How to connect using API

JSON SEND

    {
      'email':'exemple@exemple.com',
      'password':'exemple',
      'ipaddress':'127.0.0.1'
    }
  
### Connection possible feedback

JSON RESPONSE OK

    {
      'connected':'true',
      'nickname':'yourNickname#0000'
      'token':'yourtoken.string(255)'
    }
  
JSON RESPONSE NOK

> Email or password is not valide.

    {
      'connected':'false',
      'message':'Email or password is not valide'
    }

> Account locked for 30sec, too many try.

    {
      'connected':'false',
      'message':'Account locked for 30sec, too many try.'
    }
    
> Already loged-in

    {
      'connected':'false',
      'message':'You are already connected to the launcher, the other session has been stoped. Try to reconnect now to access to the services'
    }
    
### Other actions on API

> To acces other API, you need to send nickname and ip logged in

JSON SEND

    {
      'token':'nickname|ipaddress|token',
    }
