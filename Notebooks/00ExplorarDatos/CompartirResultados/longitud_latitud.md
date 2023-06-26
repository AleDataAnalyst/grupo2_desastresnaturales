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

SEGUNDO INTENTO

He vuelto a pasar el geopy con un bucle introduciendo excepciones para que las salte:

# geolocator = Nominatim(user_agent = "myGeocoder")
def get_location(row):
    try:
        location = geolocator.reverse((row['Latitude'], row['Longitude']))
        return location.address
    except ( SyntaxError, ValueError, AttributeError):
        return None

df_earthquake['Address'] = df_earthquake.apply(get_location, axis=1)


 el resultado es éste:
 
C:\Users\blanc\AppData\Roaming\Python\Python310\site-packages\geopy\point.py:472: UserWarning: Latitude normalization has been prohibited in the newer versions of geopy, because the normalized value happened to be on a different pole, which is probably not what was meant. If you pass coordinates as positional args, please make sure that the order is (latitude, longitude) or (y, x) in Cartesian terms.