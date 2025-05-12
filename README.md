# Ex.08 Design of Interactive Image Gallery
# Date:
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Photo Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            text-align: center;
            background-color: #f4f4f4;
            background-image: url("forest.jpg");
            background-size:cover;
            
        }

        h1 {
            margin-top: 20px;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
            padding: 20px;
        }

        .gallery img {
            width: 200px;
            height: 150px;
            border: 2px solid #ccc;
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .gallery img:hover {
            transform: scale(1.1);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal img {
            max-width: 90%;
            max-height: 90%;
            border: 4px solid white;
            border-radius: 10px;
        }

        .modal span {
            position: absolute;
            top: 20px;
            right: 40px;
            font-size: 30px;
            color: white;
            cursor: pointer;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Interactive Photo Gallery</h1>
    <div class="gallery">
        <img src="lion.jpg" alt="Image 1" onclick="openModal(this)">
        <img src="cat.jpg" alt="Image 2" onclick="openModal(this)">
        <img src="dog.jpg" alt="Image 3" onclick="openModal(this)">
        <img src="elepant.jpg" alt="Image 4" onclick="openModal(this)">
        <img src="rabbit.jpg" alt="Image 5" onclick="openModal(this)">
    </div>

    <!-- Modal for displaying larger image -->
    <div class="modal" id="imageModal">
        <span onclick="closeModal()">&times;</span>
        <img id="modalImage" src="" alt="">
    </div>

    <script>
        // Function to open the modal and display the clicked image
        function openModal(image) {
            const modal = document.getElementById('imageModal');
            const modalImg = document.getElementById('modalImage');
            modal.style.display = 'flex';
            modalImg.src = image.src;
        }

        // Function to close the modal
        function closeModal() {
            const modal = document.getElementById('imageModal');
            modal.style.display = 'none';
        }
    </script>
</body>
</html>






```

# OUTPUT:
![Screenshot 2025-05-12 184348](https://github.com/user-attachments/assets/865ef424-0e59-4599-8be6-65b7cfca40b2)
![Screenshot 2025-05-12 184355](https://github.com/user-attachments/assets/d582d431-dbcc-4afa-b9dc-fdb01c6600a5)
![Screenshot 2025-05-12 184402](https://github.com/user-attachments/assets/dfbce0e3-fef8-4221-a211-b6afe99bc92e)
![Screenshot 2025-05-12 184410](https://github.com/user-attachments/assets/83227df4-7208-4530-a120-1f3ffc7ffd21)
![Screenshot 2025-05-12 184418](https://github.com/user-attachments/assets/3792147a-8aef-43de-b7aa-01ae5e9505d4)
![Screenshot 2025-05-12 184427](https://github.com/user-attachments/assets/75394eb5-6db5-4d89-8e64-2faf0ad69b14)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
