<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">
    <title>Bootstrap Sign-Up Example</title>
</head>
<body>


<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#">Romya</a>

    
    <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
            <li class="nav-item">
                <form class="form-inline my-2 my-lg-0">
                    <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
                    <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
                </form>
            </li>
        </ul>
    </div>
</nav>


<div class="container mt-4 bg-light p-4 border border-warning">
    <h2 class="mb-4">Sign Up</h2>
    <form class="needs-validation" novalidate>
        <div class="form-row">
            <div class="form-group col-md-6">
                <label for="firstName">First Name</label>
                <input type="text" class="form-control" id="firstName" placeholder="Enter your first name" required>
                <div class="invalid-feedback">
                    Please provide your first name.
                </div>
            </div>

            <div class="form-group col-md-6">
                <label for="lastName">Last Name</label>
                <input type="text" class="form-control" id="lastName" placeholder="Enter your last name" required>
                <div class="invalid-feedback">
                    Please provide your last name.
                </div>
            </div>
        </div>

        <div class="form-group">
            <label for="email">Email</label>
            <input type="email" class="form-control" id="email" placeholder="Enter your email" required>
            <div class="invalid-feedback">
                Please provide a valid email address.
            </div>
        </div>

        <div class="form-group">
            <label for="password">Password</label>
            <input type="password" class="form-control" id="password" placeholder="Enter your password" required>
            <div class="invalid-feedback">
                Please provide a password.
            </div>
        </div>

        <div class="form-group">
            <label>Gender</label><br>
            <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="gender" id="male" value="male" required>
                <label class="form-check-label" for="male">Male</label>
            </div>
            <div class="form-check form-check-inline">
                <input class="form-check-input" type="radio" name="gender" id="female" value="female" required>
                <label class="form-check-label" for="female">Female</label>
            </div>
        </div>

        <div class="form-group">
            <div class="form-check">
                <input class="form-check-input" type="checkbox" id="terms" required>
                <label class="form-check-label" for="terms">I agree to the terms and conditions</label>
                <div class="invalid-feedback">
                    You must agree before submitting.
                </div>
            </div>
        </div>

        <button type="submit" class="btn btn-warning">Sign Up</button>
    </form>
</div>

<script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.3/dist/umd/popper.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>
<script>
   
    (function () {
        'use strict';
        window.addEventListener('load', function () {
            var forms = document.getElementsByClassName('needs-validation');
            var validation = Array.prototype.filter.call(forms, function (form) {
                form.addEventListener('submit', function (event) {
                    if (form.checkValidity() === false) {
                        event.preventDefault();
                        event.stopPropagation();
                    }
                    form.classList.add('was-validated');
                }, false);
            });
        }, false);
    })();
</script>

</body>
</html>

