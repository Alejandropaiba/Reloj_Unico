# Reloj_Unico
correr= 0
cicla= 0
nadar= 0
def setup():
    size(200, 200)
def draw():
    background(234, 195, 142)
    global correr
    global cicla
    global nadar
    circle(correr, 46, 25)
    if correr> height:
       correr= 0
    else:
     correr= map(second(), 0, 59, 0, height)
    circle(cicla, 92, 45)
    if cicla> height:
       cicla= 0
    else:
     cicla= map(minute(), 0, 59, 0, height)
    circle(nadar, 138, 65)
    if nadar> height:
       nadar= 0
    else:
     nadar= map(hour(), 0, 59, 0, height)
