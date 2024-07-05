<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact - Arsal Farrukh</title>
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <a class="navbar-brand" href="#">Arsal Farrukh</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="index.html">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="about.html">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="projects.html">Projects</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="blog.html">Blog</a>
        </li>
        <li class="nav-item active">
          <a class="nav-link" href="contact.html">Contact</a>
        </li>
      </ul>
    </div>
  </nav>
  <section id="contact" class="container mt-5">
    <h2>Contact Information</h2>
    <p>Feel free to <a href="mailto:arsalfarrukh96@gmail.com"><i class="far fa-envelope"></i> email me</a> at arsalfarrukh96@gmail.com</p>
    <p>Connect with me on LinkedIn: <a href="https://www.linkedin.com/in/your-linkedin-username" target="_blank"><i class="fab fa-linkedin"></i> Your LinkedIn Name</a></p>
    <form>
      <label for="name">Name</label>
      <input type="text" class="form-control" id="name" placeholder="Enter your name">
      <label for="email">Email address</label>
      <input type="email" class="form-control" id="email" placeholder="Enter your email">
      <label for="subject">Subject</label>
      <input type="text" class="form-control" id="subject" placeholder="Enter subject">
      <label for="message">Message</label>
      <textarea class="form-control" id="message" rows="5" placeholder="Enter your message"></textarea>
      <button type="submit" class="btn btn-primary">Submit</button>
    </form>
  </section>
  <footer class="footer mt-5 py-3 bg-dark text-white">
    <div class="container text-center">
      <p style="color: red; font-size: 1.2em;">&copy; 2024 Arsal Farrukh. Website is owned by Arsal Farrukh.</p>
    </div>
  </footer>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js"></script>
</body>
</html>
