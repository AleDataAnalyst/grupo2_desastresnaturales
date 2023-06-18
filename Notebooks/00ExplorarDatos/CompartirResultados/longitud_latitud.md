Cuando la notación de longitud y latitud lleva letras (latitud N o S o longitud W o E p.e)el programa geolocator no lo coge. Modificar esos valores.

latitude = 48.60 N
longitude = 58.00 W

geolocator = Nominatim(user_agent = "MozillaFirefox")
location = geolocator.reverse([latitude, longitude])
print(location.address)

 Cell In[82], line 1
    latitude = 48.60 N
                     ^
SyntaxError: invalid syntax


latitude = -36.305	
longitude = -72.315

geolocator = Nominatim(user_agent = "MozillaFirefox")
location = geolocator.reverse([latitude, longitude])
print(location.address)

Ruta N-70-M, Torrecillas, Ninhue, Provincia de Itata, Región de Ñuble, Chile