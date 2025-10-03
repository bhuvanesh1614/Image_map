# Ex04 Places Around Me
# Date:3-10-2025
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
```{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            background-image: linear-gradient(90deg,rgb(10, 185, 220),rgb(244, 39, 244),rgb(219, 211, 211));
        }
    </style>
</head>
<body>
    <center>
        <image src="{% static 'map2.png' %}"  usemap="#image-map" alt="Chennai Map" height="800" width="1400"><br>
    
    </center>
    <map name="image-map">
        <area title="ITC-limited" href="{% url 'i' %}" coords="472,250,623,249,465,322,612,312" shape="poly">
        <area title="MRF tyre factory" href="{% url 'mr' %}" coords="593,531,770,510,744,567,599,588" shape="poly">
        <area title="Royal-enfield" href="{% url 'ro' %}" coords="415,668,574,672,549,735,430,728" shape="poly">
        <area title="Wimconagar Metro" href="{% url 'me' %}" coords="477,472,629,481,582,554,474,532" shape="poly">
        <area title="Wimcorailway station" href="{% url 'ra' %}" coords="493,364,650,360,635,437,505,414" shape="poly">
    </map>
    
</body>
</html>
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <style>
        body{
            background-color:khaki;
        }
        img{
            width:1200px;
            height:500px;
            border-radius: 20px;
        }
        p{
            text-align: justify;
            line-height: 1.5;
            padding: 20px;
        }
        h1{
            color: rgb(248, 16, 54);
        }
    </style>
</head>
<body>
    <center>
        <h1>ITC-limited</h1>
         <image src="{% static 'itc.png' %}" height="400" width="400"><br>
    </center>
    <p><i>
        The ITC unit at Wimco Nagar, Tiruvottiyur (Chennai) is part of ITC’s Printing & Packaging 
        division. It manufactures folding cartons, laminates, and flexible films for various FMCG 
        products. Located near Wimco Nagar railway station, this unit is an important industrial 
        hub and provides local employment. ITC has also introduced sustainable practices here, 
        including wind energy usage for captive power.
        The facility includes staff quarters and housing for workers, making it a self-contained 
        industrial campus. It is one of ITC’s key printing and packaging centers in South India.
         ITC is well-known for its cigarettes and tobacco products, but its non-tobacco businesses 
         like packaged foods, personal care, and lifestyle products have grown significantly, 
         making it a major contributor to India’s economy. The company emphasizes sustainability and rural development,
          supporting farmers and eco-friendly initiatives. With a strong brand presence and wide-ranging business 
          operations, ITC has become one of India’s most respected and diversified conglomerates.
          </i>

    </p>

    
</body>
</html>
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <style>
        body{
            background-color:rgb(60, 231, 174);
        }
        img{
            width:1200px;
            height:500px;
            border-radius: 20px;
        }
        p{
            text-align: justify;
            line-height: 1.5;
            padding: 20px;
        }
        h1{
            color: rgb(173, 209, 28);
        }

    </style>
</head>
<body>
    <center>
        <h1>Wimco nagar Railway Station</h1>
         <image src="{% static 'wimco.png' %}" height="400" width="400"><br>
    </center>
    <p><i>
        Wimco Nagar railway station (WCN) is a suburban station in Tiruvottiyur, North Chennai, 
        located about 11 km from Chennai Central. It lies on the Chennai Central–
        Gummidipoondi line and mainly serves daily commuters from Wimco Nagar and nearby 
        areas. The station was electrified in 1979 and has basic facilities including parking.
        an important role in connecting the northern suburbs with the city. Recently, it has been 
        identified for development into a major transport hub, integrating suburban rail, metro.
        Wimco Nagar Metro Station is an elevated terminus on Line 1 of Chennai Metro's Blue Line, 
        inaugurated on 14 February 2021 as part of the northern extension of Phase I.
        Situated in the Tiruvottiyur locality, approximately 600 meters from the coast,
        it serves as a crucial transit point for the northern suburbs of Chennai .
        </i>



    </p>

    
</body>
</html>
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <style>
        body{
            background-color:rgb(24, 185, 225);
        }
        img{
            width:1200px;
            height:500px;
            border-radius: 20px;
        }
        p{
            text-align: justify;
            line-height: 1.5;
            padding: 20px;
        }
        h1{
            color: rgb(232, 146, 16);
        }
    </style>
</head>
<body>
    <center>
        <h1>Wimco nagar Metro Station</h1>
         <image src="{% static 'metro.png' %}" height="400" width="400"><br>
    </center>
    <p><i>
        Wimco Nagar Metro Station is an elevated terminal station on the Blue Line of Chennai 
        Metro, opened in February 2021. Located in Tiruvottiyur, North Chennai, it connects the 
        northern suburbs with central and southern parts of the city. The station has modern 
        facilities like lifts, escalators, and parking, and it lies close to Wimco Nagar railway station, 
        offering good multi-mode connectivity.
        It also houses a nearby metro depot, making it an important hub for operations 
        and future city transport development.
        </i>
    </p>

    
</body>
</html>
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <style>
        body{
            background-color:rgb(169, 26, 174);
        }
        img{
            width:1200px;
            height:500px;
            border-radius: 20px;
        }
        p{
            text-align: justify;
            line-height: 1.5;
            padding: 20px;
        }
        h1{
            color: rgb(227, 17, 143);
        }
    </style>
</head>
<body>
    <center>
        <h1>MRF Tyre Factory</h1>
        <image src="{% static 'mrf.png' %}" height="400" width="400"><br>
    </center>
    <p><i>
        MRF’s facility at Wimco Nagar, Tiruvottiyur (North Chennai) is one of the major tire 
        manufacturing plants of Madras Rubber Factory (MRF). Established decades ago, it has been a key contributor to MRF’s growth 
        as India’s leading tire brand. The plant produces a wide range of tires for cars, trucks, 
        and two-wheelers, supplying both domestic and international markets. Situated near Wimco Nagar railway
         and metro stations, the factory provides significant local employment and 
         stands as an important industrial landmark of the area.
         MRF produces a wide range of tires for motorcycles, cars, trucks, and buses, and is recognized for its quality,
          durability, and performance. The company also has a strong presence in motorsports,
           which helps test and showcase its products. Over the years, MRF has become a symbol of innovation
            and reliability in the Indian automotive industry.


         </i>
        
    </p>

    
</body>
</html>
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
    <style>
        body{
            background-color:rgb(233, 38, 38);
        }
        img{
            width:1200px;
            height:500px;
            border-radius: 20px;
        }
        p{
            text-align: justify;
            line-height: 1.5;
            padding: 20px;
        }
        h1{
            color: rgb(47, 17, 218);
        }
    </style>
</head>
<body>
    <center>
        <h1>Royal Enfield</h1>
        <image src="{% static 'royal.png' %}" height="400" width="400"><br>
    </center>
    <p>
        <i>Royal Enfield’s plant at Tiruvottiyur (Wimco Nagar, North Chennai) is one of the company’s 
        oldest manufacturing facilities. Established in 1955, it was here that the iconic Bullet motorcycles began production in India. 
        The factory played a major role in building Royal Enfield’s legacy and still operates as part of the brand’s network, 
        though larger new plants have since come up in Oragadam and Vallam Vadagal. Located close to Wimco Nagar railway 
        and metro stations, it remains a landmark industrial site in North Chennai.
        in Chennai and gradually expanded into rubber products and tire manufacturing. Today, MRF produces a wide range of tires 
        for motorcycles, cars, trucks, buses, and off-road vehicles, known for their durability, performance, and reliability. 
        Beyond tires, the company also manufactures conveyor belts, paints, and other rubber-based products. 
        MRF has a strong presence in motorsports, sponsoring and participating in various racing events,
         which helps showcase the performance of its products under extreme conditions.
        </i>
        
    </p>

    
</body>
</html>
```
# OUTPUT
![alt text](<Screenshot 2025-10-03 123339.png>)
![alt text](<Screenshot 2025-10-03 123409.png>)
![alt text](<Screenshot 2025-10-03 123442.png>)
![alt text](<Screenshot 2025-10-03 123506.png>)
![alt text](<Screenshot 2025-10-03 123530.png>)
![alt text](<Screenshot 2025-10-03 123559.png>)
# RESULT
The program for implementing image maps using HTML is executed successfully.
