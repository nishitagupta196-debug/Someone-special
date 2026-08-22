<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Anjeet 🎂</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    min-height: 100vh;
    overflow: hidden;
    font-family: "Trebuchet MS", sans-serif;
    background: linear-gradient(135deg, #fff1f5, #ffe4ec, #fff8fa);
    display: flex;
    justify-content: center;
    align-items: center;
}

/* Main screen */
.scene {
    width: 100%;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
}

/* ---------------- ENVELOPE ---------------- */

.envelope-area {
    display: flex;
    flex-direction: column;
    align-items: center;
    transition: 1s ease;
}

.instruction {
    color: #9d526d;
    font-size: 18px;
    margin-bottom: 25px;
    animation: fadeText 2s infinite alternate;
}

@keyframes fadeText {
    from { opacity: .5; }
    to { opacity: 1; }
}

.envelope {
    width: 280px;
    height: 190px;
    position: relative;
    cursor: pointer;
    animation: gentleMove 2.5s ease-in-out infinite;
    filter: drop-shadow(0 15px 18px rgba(180, 105, 130, .25));
}

@keyframes gentleMove {
    0%, 100% {
        transform: translateX(-7px) rotate(-1deg);
    }
    50% {
        transform: translateX(7px) rotate(1deg);
    }
}

/* Envelope body */
.envelope-body {
    position: absolute;
    width: 100%;
    height: 100%;
    background: #f7d1dc;
    border-radius: 10px;
    border: 2px solid #e7aebe;
    overflow: hidden;
}

/* Lower triangular folds */
.envelope-body::before {
    content: "";
    position: absolute;
    bottom: 0;
    left: 0;
    border-left: 140px solid transparent;
    border-right: 140px solid transparent;
    border-bottom: 105px solid #efbdcd;
    z-index: 2;
}

/* Top flap */
.flap {
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 0;
    border-left: 140px solid transparent;
    border-right: 140px solid transparent;
    border-top: 105px solid #f
