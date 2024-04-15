# Week 1: Introduction to Deep Learning

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Progress Bar Example</title>
<style>
    .progress-container {
        width: 100%;
        background-color: #f3f3f3;
    }

    .progress-bar {
        width: 0%;
        height: 30px;
        background-color: #4caf50;
        text-align: center;
        line-height: 30px;
        color: white;
    }
</style>
</head>
<body>

<div class="progress-container">
  <div class="progress-bar" id="myBar">0%</div>
</div>

<script>
// Simulate progress by increasing the width of the progress bar
let width = 0;
const progressBar = document.getElementById("myBar");

function increaseProgress() {
    if (width >= 100) {
        clearInterval(progressInterval);
    } else {
        width++;
        progressBar.style.width = width + "%";
        progressBar.innerHTML = width + "%";
    }
}

// Interval to increase progress every 50 milliseconds (adjust as needed)
const progressInterval = setInterval(increaseProgress, 50);
</script>

</body>
</html>

