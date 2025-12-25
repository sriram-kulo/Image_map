# Ex04 Places Around Me
# Date:
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE
```
home.html
<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Map</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: black;
        }
       
</style>
</head>
<body>
    {% load static %}
    <h1 style="text-align: center; color: white;">THIRUVOOTIYUR</h1>
    <h2 style="text-align: center; color: white;">BARATH B 25009091</h2>
<img src="{% static 'map.png' %}" usemap="#image-map" style="display: block;width: 100%; height: auto;">

<map name="image-map">
    <area  alt="kailash sector " title="kailash sector " href="kailash.html" coords="920,387,980,420" shape="rect">
    <area  alt="odiyam mani " title="odiyam mani " href="om.html" coords="500,550,600,700" shape="rect">
    <area  alt="metro" title="metro" href="metro.html" coords="1050,90,1130,140" shape="rect">
    <area  alt="our lady school" title="our lady school" href="school.html" coords="1000,400,1100,500" shape="rect">
    <area  alt="thiruvootiyur railway" title="thiruvootiyur railway" href="rail.html" coords="600,140,650,240" shape="rect">
</map>
</html>

kailash.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
    <title>Map</title>
    <style>

body {
  font-family: 'MyFont', sans-serif;
}
.ani {
    transition: all 2s ease;
  }



  </style>
</head>
<body style="background-color:black ; overflow:hidden;">
  <div id="circle" style="position:absolute; left: 800px; top:30px; width:367px; height:367px; background-color:black; border: 5px solid white;" class="ani"> </div>
    <img  id= "pfp" src="{% static 'kailash.png' %}" style="position:absolute; left: 970px; top: 66px; width: 367px;height: 367px; border: 8px solid white;" class="ani">
    <p style="position:absolute; left: 70px; top: 100px; color:white; font-size:70px;" class="ani">
      KAILASH SECTOR
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 300px; color:white; font-size:24px; width:800px;" class="ani">
      kailash sector is a colony <br> many houses live inside this<br> it is maintaied good and clean
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 500px; color:white; font-size:24px; width:800px;" class="ani">
      Kailash Sector<br>
கைலாஷ் செக்டார்<br>
Tiruvottiyur<br>
Chennai, Tamil Nadu 600019
    </p>

    <a href="home.html">
  <button style="position: absolute;width: 447px;height: 111px;left: 800px;top: 500px;background: #D9D9D9;border-radius: 50px;font-size: 40px;">back to map</button>
</a>

</body>
</html>

metro.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
    <title>Map</title>
    <style>

body {
  font-family: 'MyFont', sans-serif;
}
.ani {
    transition: all 2s ease;
  }



  </style>
</head>
<body style="background-color:black ; overflow:hidden;">
  <div id="circle" style="position:absolute; left: 800px; top:30px; width:367px; height:367px; background-color:black; border: 5px solid white;" class="ani"> </div>
    <img  id= "pfp" src="{% static 'metro.png' %}" style="position:absolute; left: 970px; top: 66px; width: 367px;height: 367px; border: 8px solid white;" class="ani">
    <p style="position:absolute; left: 70px; top: 100px; color:white; font-size:70px;" class="ani">
      METRO
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 300px; color:white; font-size:24px; width:800px;" class="ani">
      this ia metro station <br>it connects to most cities<br>it is easy and convient for travelling
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 500px; color:white; font-size:24px; width:800px;" class="ani">
      Rajakadai, Tiruvottiyur,<br> Chennai, Tamil Nadu 600019
    </p>
    <a href="home.html">
  <button style="position: absolute;width: 447px;height: 111px;left: 800px;top: 500px;background: #D9D9D9;border-radius: 50px;font-size: 40px;">back to map</button>
</a>

</body>
</html>

om.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
    <title>Map</title>
    <style>

body {
  font-family: 'MyFont', sans-serif;
}
.ani {
    transition: all 2s ease;
  }



  </style>
</head>
<body style="background-color:black ; overflow:hidden;">
  <div id="circle" style="position:absolute; left: 800px; top:30px; width:367px; height:367px; background-color:black; border: 5px solid white;" class="ani"> </div>
    <img  id= "pfp" src="{% static 'om.png' %}" style="position:absolute; left: 970px; top: 66px; width: 367px;height: 367px; border: 8px solid white;" class="ani">
    <p style="position:absolute; left: 70px; top: 100px; color:white; font-size:70px;" class="ani">
      ODIYAM MANI 
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 300px; color:white; font-size:24px; width:800px;" class="ani">
      this is a local theatre<br> it is one that local people uses<br> it telecats popular movies
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 500px; color:white; font-size:24px; width:800px;" class="ani">
      573W+G77, W Mada St, Kaladipet,<br> Tiruvottiyur, <br>Chennai, Tamil Nadu 600019
    </p>

    <a href="home.html">
  <button style="position: absolute;width: 447px;height: 111px;left: 800px;top: 500px;background: #D9D9D9;border-radius: 50px;font-size: 40px;">back to map</button>
</a>

</body>
</html>

rail.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
    <title>Map</title>
    <style>

body {
  font-family: 'MyFont', sans-serif;
}
.ani {
    transition: all 2s ease;
  }



  </style>
</head>
<body style="background-color:black ; overflow:hidden;">
  <div id="circle" style="position:absolute; left: 800px; top:30px; width:367px; height:367px; background-color:black; border: 5px solid white;" class="ani"> </div>
    <img  id= "pfp" src="{% static 'rail.png' %}" style="position:absolute; left: 970px; top: 66px; width: 367px;height: 367px; border: 8px solid white;" class="ani">
    <p style="position:absolute; left: 70px; top: 100px; color:white; font-size:70px;" class="ani">
    RAILWAY STATION
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 300px; color:white; font-size:24px; width:800px;" class="ani">
      this is a railway station<br> many people use this transport<br> a local transport <br> for travelling
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 500px; color:white; font-size:24px; width:800px;" class="ani">
     KCP Rd, Tiruvottiyur, Chennai, <br>Tamil Nadu 600019<br> contact:09677054301
    </p>
    <a href="home.html">
  <button style="position: absolute;width: 447px;height: 111px;left: 800px;top: 500px;background: #D9D9D9;border-radius: 50px;font-size: 40px;">back to map</button>
</a>

</body>
</html>

school.html

<!DOCTYPE html>
<html lang="en">
{% load static %}
<head>
    <title>Map</title>
    <style>

body {
  font-family: 'MyFont', sans-serif;
}
.ani {
    transition: all 2s ease;
  }



  </style>
</head>
<body style="background-color:black ; overflow:hidden;">
  <div id="circle" style="position:absolute; left: 800px; top:30px; width:367px; height:367px; background-color:black; border: 5px solid white;" class="ani"> </div>
    <img  id= "pfp" src="{% static 'school.png' %}" style="position:absolute; left: 970px; top: 66px; width: 367px;height: 367px; border: 8px solid white;" class="ani">
    <p style="position:absolute; left: 70px; top: 100px; color:white; font-size:70px;" class="ani">
      OUR LADY SCHOOL
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 300px; color:white; font-size:24px; width:800px;" class="ani">
      OUR LADY SCHOOL <br> THIS SCHOOL HAS LKG -12TH<br> ONE OF BEST SCHOOL FOR SPORTS<br> AND ALSO FOR STUDIES
    </p>
    <p id="details" style="position:absolute; left: 70px; top: 500px; color:white; font-size:24px; width:800px;" class="ani">
      Thiruvottiyur High Rd, Sathiyamoorthy Nagar,<br> Rajakadai, Tiruvottiyur, Chennai, Tamil Nadu 600019
    </p>

    <a href="home.html">
  <button style="position: absolute;width: 447px;height: 111px;left: 800px;top: 500px;background: #D9D9D9;border-radius: 50px;font-size: 40px;">back to map</button>
</a>

</body>
</html>
```
# OUTPUT
<img width="1920" height="1080" alt="SRIRAM M 25000692" src="https://github.com/user-attachments/assets/a90688a9-61e5-4552-9817-a4c6a6b616c2" />
<img width="1917" height="1079" alt="528686705-9acdf1ab-63ce-4056-a21c-a0ddfa26440b" src="https://github.com/user-attachments/assets/ab8d14a9-7657-4d99-8681-3221d04b2fd5" />

# RESULT
The program for implementing image maps using HTML is executed successfully.
