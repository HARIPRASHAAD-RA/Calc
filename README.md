# Ex.08 Design of a Standard Calculator
## Date:06-05-2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <script src="script.js"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.4/jquery.min.js"></script>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
    <script>
    function calculatorbtns(e) {
        if (e.innerHTML == '=') {
            result.value = eval(result.value);
        }
        else if (e.id == 'back') {
            v = result.value;
            result.value = v.substring(0, v.length - 1);
        }
        else if (e.innerHTML == 'C') {
            result.value = '';
        }
        else {
            result.value += e.innerHTML;
        }
    }
</script>
</head>

<body style="background-color: rgb(208, 208, 208);">
    <div id="fulldiv">
        <textarea id="result" type="number" placeholder="Calculator"></textarea>
        <br>
        <button class="btns" onclick="calculatorbtns(this)">7</button>
        <button class="btns" onclick="calculatorbtns(this)">8</button>
        <button class="btns" onclick="calculatorbtns(this)">9</button>
        <button class="btns1" onclick="calculatorbtns(this)">/</button>
        <button class="btns1" id="back" onclick="calculatorbtns(this)"><i class="bi bi-backspace"></i></button>
        <br>
        <button class="btns" onclick="calculatorbtns(this)">4</button>
        <button class="btns" onclick="calculatorbtns(this)">5</button>
        <button class="btns" onclick="calculatorbtns(this)">6</button>
        <button class="btns1" onclick="calculatorbtns(this)">X</button>
        <button class="btns1"  onclick="calculatorbtns(this)">rt</button>
        <br>
        <button class="btns" onclick="calculatorbtns(this)">1</button>
        <button class="btns" onclick="calculatorbtns(this)">2</button>
        <button class="btns" onclick="calculatorbtns(this)">3</button>
        <button class="btns1" onclick="calculatorbtns(this)">-</button>
        <button class="btns1" onclick="calculatorbtns(this)">%</button>
        <br>
        <button class="btns" onclick="calculatorbtns(this)">0</button>
        <button class="btns" onclick="calculatorbtns(this)">.</button>
        <button id="btnc" class="btns" onclick="calculatorbtns(this)">C</button>
        <button class="btns1" onclick="calculatorbtns(this)">+</button>
        <button class="btns1" onclick="calculatorbtns(this)">=</button>
    </div>
</body>

</html>
```
## OUTPUT:
![image](https://github.com/HARIPRASHAAD-RA/Calc/assets/164654451/3c2a2834-9410-48c1-92b1-d10bf088fb24)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
