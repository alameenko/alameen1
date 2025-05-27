# alameen1<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>My Personal Website</title>
  <style>
    body { font-family: Arial; text-align: center; padding: 20px; }
    .card { margin-top: 30px; padding: 20px; border: 1px solid #ccc; border-radius: 10px; display: inline-block; }
  </style>
</head>
<body>
  <h1>Welcome to My Website</h1>
  <div class="card">
    <p><strong>Name:</strong> Your Name</p>
    <p><strong>Email:</strong> your@email.com</p>
    <a href="cv.pdf" download><button>Download My CV</button></a>
    <br><br>
    <input type="file" id="uploadCV" />
    <p><em>(Uploads won't be saved on GitHub Pages — for demo only)</em></p>
  </div>

  <script>
    document.getElementById('uploadCV').addEventListener('change', function() {
      const file = this.files[0];
      if (file) {
        alert(`Uploaded: ${file.name}\n(Note: Not actually stored. Just demo.)`);
      }
    });
  </script>
</body>
</html>
