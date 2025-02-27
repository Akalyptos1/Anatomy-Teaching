# Anatomy-Teaching
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spinal Anatomy Quiz</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="quiz-container">
        <h2 id="question">Loading question...</h2>
        <img id="question-image" src="" alt="Anatomy Image">
        <ul id="options-list"></ul>
        <h3 id="final-score" style="display: none;"></h3>
    </div>
    <script src="script.js"></script>
</body>
</html>

body {
    font-family: 'Arial', sans-serif;
    text-align: center;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
}
.quiz-container {
    width: 80%;
    max-width: 600px;
    margin: 20px auto;
    padding: 20px;
    border-radius: 10px;
    background-color: white;
    box-shadow: 3px 3px 15px rgba(0, 0, 0, 0.2);
}
#question-image {
    width: 100%;
    max-width: 500px;
    border-radius: 5px;
}
ul {
    list-style: none;
    padding: 0;
}
li {
    padding: 10px;
    
const quizData = [
    { question: "Identify the structure shown:", image: "https://i.imgur.com/SHPhuF1.png", options: ["The C1 Vertebra - Atlas", "The C2 Vertebra - Axis", "Cervical vertebra", "Thoracic Vertebrae"], answer: "The C1 Vertebra - Atlas" },
    { question: "Identify the structure shown:", image: "https://i.imgur.com/maAjJQP.png", options: ["The C1 Vertebra - Atlas", "The C2 Vertebra - Axis", "Cervical vertebra", "Thoracic Vertebrae"], answer: "The C2 Vertebra - Axis" },
    { question: "Identify the structure shown:", image: "https://i.imgur.com/AJxFHJd.png", options: ["Atypical Cervical Vertebrae", "Typical Cervical Vertebrae", "Typical Thoracic Vertebrae", "Typical Lumbar Vertebrae"], answer: "Typical Cervical Vertebrae" },
    { question: "Identify the structure shown:", image: "https://i.imgur.com/6gZjgqL.png", options: ["Typical Cervical Vertebrae", "Atypical Cervical Vertebrae", "Typical Thoracic Vertebrae", "Typical Lumbar Vertebrae"], answer: "Typical Lumbar Vertebrae" },
    { question: "Identify the covered structure:", image: "https://i.imgur.com/98WceP8.png", options: ["Anterior Sacral Foramina", "Articular Surface for Lumbosacral Joint", "Posterior Sacral Foramina", "Ala"], answer: "Articular Surface for Lumbosacral Joint" },
    { question: "Identify the missing structure:", image: "https://i.imgur.com/50hZB0a.png", options: ["Ala", "Sacral Hiatus", "Posterior Sacral Foramina", "Superior Articular Process"], answer: "Ala" },
    { question: "Identify the correct name for the structures shown:", image: "https://i.imgur.com/LZJSRaP.png", options: ["Anterior Sacral Foramina", "Posterior Sacral Foramina", "Articular Surface for Lumbosacral Joint", "Superior Articular Process"], answer: "Posterior Sacral Foramina" },
    { question: "Identify the ligament indicated by the arrow:", image: "https://i.imgur.com/LU4e1Vv.png", options: ["Laminous Ligament", "Intervertebral Disc", "Ligament Flavum", "Interspinous Ligament"], answer: "Ligament Flavum" },
    { question: "Identify the ligament indicated by the arrow:", image: "https://i.imgur.com/rFycANN.png", options: ["Supraspinous Ligament", "Ligament Flavum", "Intervertebral Disc", "Interspinous Ligament"], answer: "Supraspinous Ligament" },
    { question: "Identify the ligament indicated by the arrow:", image: "https://i.imgur.com/kQIx82Q.png", options: ["Supraspinous Ligament", "Ligament Flavum", "Ligamentum Nuchae", "Interspinous Ligament"], answer: "Ligamentum Nuchae" },
    { question: "Identify the ligament indicated by the arrow:", image: "https://i.imgur.com/W4ZwTKv.png", options: ["Interspinous Ligament", "Laminous Ligament", "Anterior Longitudinal Ligament", "Ligament Flavum"], answer: "Anterior Longitudinal Ligament" },
    { question: "Identify the muscle group indicated by the arrow:", image: "https://i.imgur.com/NfqW8yY.png", options: ["Spinalis", "Rhomboid Minor", "Latissimus Dorsi", "Rhomboid Major"], answer: "Rhomboid Minor" },
    { question: "Identify the muscle group indicated by the arrow:", image: "https://i.imgur.com/hbjvFdi.png", options: ["Spinalis", "Trapezius", "Levator Scapulae", "Latissimus Dorsi"], answer: "Latissimus Dorsi" },
    { question: "Identify the muscle group indicated by the arrow:", image: "https://i.imgur.com/urwT8UC.png", options: ["Levator Scapulae", "Rhomboid Major", "Trapezius", "Rhomboid Minor"], answer: "Levator Scapulae" },