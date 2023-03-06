# CSS

# Transicions - Exemple

![image](https://user-images.githubusercontent.com/110727546/223174612-541213a4-209f-4d3f-90cc-6af089cb0fd3.png)

![image](https://user-images.githubusercontent.com/110727546/223174574-2b557c95-476c-4f97-addd-82f6aa6b4f01.png)

```
<!DOCTYPE html>
<html>
<head>
<style> 
.animated_div {
    width: 60px;
    height: 40px;
    background: #92B901;
    color: #ffffff;
    position: absolute;
    font-weight: bold;
    font-size: 15px;
    padding: 10px;
    float: left;
    margin: 5px;   
    transition-property: width,height,transform,background,font-size,opacity;
    transition-duration: 1s,1s,1s,1s,1s,1s;
    border-radius: 5px;
    opacity: 0.4;
}
.animated_div:hover
{
opacity:1;
background:#1ec7e6;
width:130px;
height:80px;
font-size:35px;
}
</style>
</head>
<body>

<h1>The transition Property</h1>

<p>Hover over the div element below, to see the transition effect:</p>
<div class="animated_div"> CSS</div>

</body>
</html>
```
