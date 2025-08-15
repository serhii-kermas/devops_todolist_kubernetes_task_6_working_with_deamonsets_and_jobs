kubectl apply -f namespace.yml
kubectl apply -f clusterIp.yml
kubectl apply -f deployment.yml
kubectl apply -f daemonset.yml
kubectl apply -f cronjob.yml

<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Basic Page Needs
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta charset="utf-8">
  <title>Djodolist</title>
  <meta name="description" content="Small todolist app.">
  <meta name="author" content="Christian Rotzoll">
  <!-- Mobile Specific Metas
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link href='http://fonts.googleapis.com/css?family=Raleway:400,300,600' rel='stylesheet' type='text/css'>
  
  <!-- CSS
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/normalize/3.0.2/normalize.min.css">;
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css">;
  <link rel="stylesheet" type='text/css' href="/static/css/custom.css">
  
  <!-- Scripts
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>;
  <script type="text/javascript" src="/static/js/site.js"></script>
  
  <!-- Favicon
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="icon" type="image/png" href="/static/images/favicon.png" />
</head>
<body>
  <!-- Primary Page Layout
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <div class="container">
    <!-- Navigation
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <div class="navbar-spacer"></div>
    <nav class="navbar">
      <div class="container">
        <ul class="navbar-list">
          <li class="navbar-item"><a class="navbar-link" href="/">Djodolist</a></li>
          
          <li class="navbar-item">
            <a class="navbar-link" href="/auth/login/">Login</a> 
        </ul>
      </div>
    </nav>
    
<section class="header">
  <h2 class="title">Dead simple Todolists.</h2>
  <div class="row">
    <div class="three columns value-prop"></div>
    <div class="six columns">
      <form action="/todolist/new/" method=post>
        <input type="hidden" name="csrfmiddlewaretoken" value="CjMpI6Sv3rsrPD4pN51OKCC7VthczRA1lAZT3Q1Dm0mYWDYeGOgmriJPkIco05nZ">
        <dl>
          <dd><tr>
    <th></th>
    <td>
      
      <input type="text" name="description" class="u-full-width" placeholder="Enter your todo" maxlength="128" required id="id_description">
      
      
        
      
    </td>
  </tr>
          <dt><input type="submit" class="button button-primary" value="Start one now">
        </dl>
      </form>
    </div>
  </div>
</section>
  </div>
  <!-- End Document
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
</body>
</html>

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100  3747  100  3747    0     0  18635      0 --:--:-- --:--:-- --:--:-- 37848
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Basic Page Needs
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta charset="utf-8">
  <title>Djodolist</title>
  <meta name="description" content="Small todolist app.">
  <meta name="author" content="Christian Rotzoll">
  <!-- Mobile Specific Metas
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link href='http://fonts.googleapis.com/css?family=Raleway:400,300,600' rel='stylesheet' type='text/css'>
  
  <!-- CSS
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/normalize/3.0.2/normalize.min.css">;
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css">;
  <link rel="stylesheet" type='text/css' href="/static/css/custom.css">
  
  <!-- Scripts
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>;
  <script type="text/javascript" src="/static/js/site.js"></script>
  
  <!-- Favicon
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="icon" type="image/png" href="/static/images/favicon.png" />
</head>
<body>
  <!-- Primary Page Layout
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <div class="container">
    <!-- Navigation
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <div class="navbar-spacer"></div>
    <nav class="navbar">
      <div class="container">
        <ul class="navbar-list">
          <li class="navbar-item"><a class="navbar-link" href="/">Djodolist</a></li>
          
          <li class="navbar-item">
            <a class="navbar-link" href="/auth/login/">Login</a> 
        </ul>
      </div>
    </nav>
    
<section class="header">
  <h2 class="title">Dead simple Todolists.</h2>
  <div class="row">
    <div class="three columns value-prop"></div>
    <div class="six columns">
      <form action="/todolist/new/" method=post>
        <input type="hidden" name="csrfmiddlewaretoken" value="tt9ja170c0SfHqfiCHOAISEPFj3Vy41RLB6VAtRvCBFvWBbv2u65eeMY5BchVi48">
        <dl>
          <dd><tr>
    <th></th>
    <td>
      
      <input type="text" name="description" class="u-full-width" placeholder="Enter your todo" maxlength="128" required id="id_description">
      
      
        
      
    </td>
  </tr>
          <dt><input type="submit" class="button button-primary" value="Start one now">
        </dl>
      </form>
    </div>
  </div>
</section>
  </div>
  <!-- End Document
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
</body>
</html>

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100  3747  100  3747    0     0  18594      0 --:--:-- --:--:-- --:--:-- 37848
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Basic Page Needs
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta charset="utf-8">
  <title>Djodolist</title>
  <meta name="description" content="Small todolist app.">
  <meta name="author" content="Christian Rotzoll">
  <!-- Mobile Specific Metas
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link href='http://fonts.googleapis.com/css?family=Raleway:400,300,600' rel='stylesheet' type='text/css'>
  
  <!-- CSS
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/normalize/3.0.2/normalize.min.css">;
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css">;
  <link rel="stylesheet" type='text/css' href="/static/css/custom.css">
  
  <!-- Scripts
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>;
  <script type="text/javascript" src="/static/js/site.js"></script>
  
  <!-- Favicon
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="icon" type="image/png" href="/static/images/favicon.png" />
</head>
<body>
  <!-- Primary Page Layout
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <div class="container">
    <!-- Navigation
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <div class="navbar-spacer"></div>
    <nav class="navbar">
      <div class="container">
        <ul class="navbar-list">
          <li class="navbar-item"><a class="navbar-link" href="/">Djodolist</a></li>
          
          <li class="navbar-item">
            <a class="navbar-link" href="/auth/login/">Login</a> 
        </ul>
      </div>
    </nav>
    
<section class="header">
  <h2 class="title">Dead simple Todolists.</h2>
  <div class="row">
    <div class="three columns value-prop"></div>
    <div class="six columns">
      <form action="/todolist/new/" method=post>
        <input type="hidden" name="csrfmiddlewaretoken" value="35hBP4kAOrDFnW8ItVfFB0OGFcBHMLInpJH6wbrOs8O1QyaSc0dOhebMCoTYggds">
        <dl>
          <dd><tr>
    <th></th>
    <td>
      
      <input type="text" name="description" class="u-full-width" placeholder="Enter your todo" maxlength="128" required id="id_description">
      
      
        
      
    </td>
  </tr>
          <dt><input type="submit" class="button button-primary" value="Start one now">
        </dl>
      </form>
    </div>
  </div>
</section>
  </div>
  <!-- End Document
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
</body>
</html>

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100  3747  100  3747    0     0  32702      0 --:--:-- --:--:-- --:--:-- 39031

  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Basic Page Needs
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta charset="utf-8">
  <title>Djodolist</title>
  <meta name="description" content="Small todolist app.">
  <meta name="author" content="Christian Rotzoll">
  <!-- Mobile Specific Metas
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link href='http://fonts.googleapis.com/css?family=Raleway:400,300,600' rel='stylesheet' type='text/css'>
  
  <!-- CSS
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/normalize/3.0.2/normalize.min.css">;
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css">;
  <link rel="stylesheet" type='text/css' href="/static/css/custom.css">
  
  <!-- Scripts
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>;
  <script type="text/javascript" src="/static/js/site.js"></script>
  
  <!-- Favicon
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="icon" type="image/png" href="/static/images/favicon.png" />
</head>
<body>
  <!-- Primary Page Layout
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <div class="container">
    <!-- Navigation
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <div class="navbar-spacer"></div>
    <nav class="navbar">
      <div class="container">
        <ul class="navbar-list">
          <li class="navbar-item"><a class="navbar-link" href="/">Djodolist</a></li>
          
          <li class="navbar-item">
            <a class="navbar-link" href="/auth/login/">Login</a> 
        </ul>
      </div>
    </nav>
    
<section class="header">
  <h2 class="title">Dead simple Todolists.</h2>
  <div class="row">
    <div class="three columns value-prop"></div>
    <div class="six columns">
      <form action="/todolist/new/" method=post>
        <input type="hidden" name="csrfmiddlewaretoken" value="425gJAwB19fNC28HDIy1Xb8Uj5XXKnPwDiN29Mb4E71O4LXcDp5Lxa4iKHl5WIsC">
        <dl>
          <dd><tr>
    <th></th>
    <td>
      
      <input type="text" name="description" class="u-full-width" placeholder="Enter your todo" maxlength="128" required id="id_description">
      
      
        
      
    </td>
  </tr>
          <dt><input type="submit" class="button button-primary" value="Start one now">
        </dl>
      </form>
    </div>
  </div>
</section>
  </div>
  <!-- End Document
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
</body>
</html>

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100  3747  100  3747    0     0  18708      0 --:--:-- --:--:-- --:--:-- 37848
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Basic Page Needs
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta charset="utf-8">
  <title>Djodolist</title>
  <meta name="description" content="Small todolist app.">
  <meta name="author" content="Christian Rotzoll">
  <!-- Mobile Specific Metas
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link href='http://fonts.googleapis.com/css?family=Raleway:400,300,600' rel='stylesheet' type='text/css'>
  
  <!-- CSS
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/normalize/3.0.2/normalize.min.css">;
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css">;
  <link rel="stylesheet" type='text/css' href="/static/css/custom.css">
  
  <!-- Scripts
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>;
  <script type="text/javascript" src="/static/js/site.js"></script>
  
  <!-- Favicon
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="icon" type="image/png" href="/static/images/favicon.png" />
</head>
<body>
  <!-- Primary Page Layout
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <div class="container">
    <!-- Navigation
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <div class="navbar-spacer"></div>
    <nav class="navbar">
      <div class="container">
        <ul class="navbar-list">
          <li class="navbar-item"><a class="navbar-link" href="/">Djodolist</a></li>
          
          <li class="navbar-item">
            <a class="navbar-link" href="/auth/login/">Login</a> 
        </ul>
      </div>
    </nav>
    
<section class="header">
  <h2 class="title">Dead simple Todolists.</h2>
  <div class="row">
    <div class="three columns value-prop"></div>
    <div class="six columns">
      <form action="/todolist/new/" method=post>
        <input type="hidden" name="csrfmiddlewaretoken" value="i98sWpdF3usmFHYLYspP9qY6jt76byGwnfaNkf3QmZqEPK4beBKLLEmO6bLZouf1">
        <dl>
          <dd><tr>
    <th></th>
    <td>
      
      <input type="text" name="description" class="u-full-width" placeholder="Enter your todo" maxlength="128" required id="id_description">
      
      
        
      
    </td>
  </tr>
          <dt><input type="submit" class="button button-primary" value="Start one now">
        </dl>
      </form>
    </div>
  </div>
</section>
  </div>
  <!-- End Document
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
</body>
</html>

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100  3747  100  3747    0     0  32684      0 --:--:-- --:--:-- --:--:-- 38628
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Basic Page Needs
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta charset="utf-8">
  <title>Djodolist</title>
  <meta name="description" content="Small todolist app.">
  <meta name="author" content="Christian Rotzoll">
  <!-- Mobile Specific Metas
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
  <!-- FONT
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link href='http://fonts.googleapis.com/css?family=Raleway:400,300,600' rel='stylesheet' type='text/css'>
  
  <!-- CSS
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/normalize/3.0.2/normalize.min.css">;
  <link rel="stylesheet" type='text/css' href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/skeleton.min.css">;
  <link rel="stylesheet" type='text/css' href="/static/css/custom.css">
  
  <!-- Scripts
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>;
  <script type="text/javascript" src="/static/js/site.js"></script>
  
  <!-- Favicon
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <link rel="icon" type="image/png" href="/static/images/favicon.png" />
</head>
<body>
  <!-- Primary Page Layout
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
  <div class="container">
    <!-- Navigation
    –––––––––––––––––––––––––––––––––––––––––––––––––– -->
    <div class="navbar-spacer"></div>
    <nav class="navbar">
      <div class="container">
        <ul class="navbar-list">
          <li class="navbar-item"><a class="navbar-link" href="/">Djodolist</a></li>
          
          <li class="navbar-item">
            <a class="navbar-link" href="/auth/login/">Login</a> 
        </ul>
      </div>
    </nav>
    
<section class="header">
  <h2 class="title">Dead simple Todolists.</h2>
  <div class="row">
    <div class="three columns value-prop"></div>
    <div class="six columns">
      <form action="/todolist/new/" method=post>
        <input type="hidden" name="csrfmiddlewaretoken" value="msytoSpFJJI3ObwNNtkgNsdE4goqp19m96yyn1d14DAoUCNFlNlbAOU114l66jAe">
        <dl>
          <dd><tr>
    <th></th>
    <td>
      
      <input type="text" name="description" class="u-full-width" placeholder="Enter your todo" maxlength="128" required id="id_description">
      
      
        
      
    </td>
  </tr>
          <dt><input type="submit" class="button button-primary" value="Start one now">
        </dl>
      </form>
    </div>
  </div>
</section>
  </div>
  <!-- End Document
  –––––––––––––––––––––––––––––––––––––––––––––––––– -->
</body>
</html>

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100  3747  100  3747    0     0  30028      0 --:--:-- --:--:-- --:--:--  121k
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
<!DOCTYPE html>
<html lang="en">
<head>
  <!-- Basic Page Needs


  Fri Aug 15 13:16:00 UTC 2025
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed

  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100     9  100     9    0     0    227      0 --:--:-- --:--:-- --:--:--   450
Health OK